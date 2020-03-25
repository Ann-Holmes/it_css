# [SVN](https://www.runoob.com/svn/svn-tutorial.html)

SVN 的全称是 subversion. 

## Ubuntu 安装

```shell
# 安装
sudo apt install subversion

# 检查是否安装成功
svn --version
```

## SVN 使用

### 一些重要的概念

- 添加的文件目录不会立刻成为版本库的一部分，而是被添加进待变更列表中，直到执行了 commit 操作后才会成为版本库的一部分。
- Rename 操作可以更改文件/目录的名字。"移动"操作用来将文件/目录从一处移动到版本库中的另一处。
- Commit 是一个原子操作，也就是说要么完全提交成功，要么失败回滚。用户不会看到成功提交一半的情况。

### SVN的启动

```bash
# 创建版本库的目录
mkdir /opt/svn

# 利用svn创建版本库
svnadmin create /opt/svn/runoob

# 使用命令svnserve启动服务
svnserve -d -r <dir> --listen-port <port>

```

- 参数 `-r` 的配置方式决定了版本库访问方式

    - `-r` 直接指定到版本库(称之为单库svnserve方式)

        ```bash
        svnserve -d -r /opt/svn/runoob
        # 在这种情况下，一个svnserve只能为一个版本库工作
        ```

    - `-r` 指定到版本库的上级目录(称之为多库svnserve方式)

        ```bash
        svnserve -d -r /opt/svn
        # 这种情况，一个svnserve可以为多个版本库工作
        ```

### SVN的配置文件

> SVN版本库创建后, 会生成如下目录: 
>
> ```bash
> conf/
> 	|__ svnserve.conf
> 	|__ passwd
> 	|__ authz
> db/
> format/
> hooks/
> locks/
> README.txt
> ```
>
> 

#### 1、svn服务配置文件svnserve.conf

```bash
# svnserve.conf
[general]
anon-access = none
auth-access = write
password-db = /home/svn/passwd # 指定 passwd 配置文件
authz-db = /home/svn/authz # 指定 authz 配置文件
realm = tiku 
```

- **anon-access:** 控制非鉴权用户访问版本库的权限，取值范围为"write"、"read"和"none"。 即"write"为可读可写，"read"为只读，"none"表示无访问权限。 默认值：read
- **auth-access:** 控制鉴权用户访问版本库的权限。取值范围为"write"、"read"和"none"。 即"write"为可读可写，"read"为只读，"none"表示无访问权限。 默认值：write
- **authz-db:** 指定权限配置文件名，通过该文件可以实现以路径为基础的访问控制。 除非指定绝对路径，否则文件位置为相对conf目录的相对路径。 默认值：authz
- **realm:** 指定版本库的认证域，即在登录时提示的认证域名称。若两个版本库的认证域相同，建议使用相同的用户名口令数据文件。 默认值：一个UUID(Universal Unique IDentifier，全局唯一标示)。

#### 2、用户名口令文件passwd

```bash
# passwd
# 格式为: <用户名> = <口令>
[users]
admin = admin
thinker = 123456
```

#### 3、权限配置文件

```bash
# authz
# [groups] 配置字段: <用户组> = <用户列表>
# 版本库路径权限端的段名格式: [<版本库名>:<路径>] 
[groups]
g_admin = admin,thinker

[admintools:/]
@g_admin = rw
* =

[test:/home/thinker]
thinker = rw
* = r
```

### SVN命令操作版本库汇总

| 命令 | 操作 |
| -- | -- |
| svn checkout <URL> --username=<user_name> --password=<passwd> | 拉去服务器的仓库到本地 |
| svn status | 列出当前版本库的状态 |
| svn add <files> | 将文件添加到版本库 | 
| svn commit -m "some useful message" | 将文件提交到版本库, 版本库的版本号更新一次 | 
| svn import <local_files/dir> <URL> --username=<user_name> --password=<passwd> | 将本地的版本库, 推送到远程仓库 | 
| svn revert <files> / svn revert -R <dir> | 回退某个文件到未修改的状态, 仅限还没有commit的文件和目录 | 
| svn merge -r num:num_before <files> / <dir> | 回退已经提交到版本库的某个文件到指定的版本(由num_before指定之前的版本) | 
| svn log | 用来展示svn 的版本作者、日期、路径等等 | 
| svn diff | 用来显示特定修改的行级详细信息 |
| svn cat | 取得在特定版本的某文件显示在当前屏幕 | 
| svn list | 显示一个目录或某一版本存在的文件 | 

