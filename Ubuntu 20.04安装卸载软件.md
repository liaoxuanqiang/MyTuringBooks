## Ubuntu 20.04安装卸载软件

### 1)安装软件

```shell
sudo apt-get install 软件名
```

### 2)卸载软件

方法一：

```shell
sudo apt-get remove 软件名
```

方法二：

```shell
sudo apt-get remove --purge 软件名
```

添加上–purge可以卸载并清除配置

### 3)卸载.deb包软件

可使用sudo dpkg -info *.deb 查看软件包信息，然后卸载方法如下：

方法一：

```shell
sudo dpkg -r *.deb
```

方法二：

```shell
sudo dpkg -r --purge *.deb
```

注意：若是想查看系统中已安装软件包信息，可以使用命令 dpkg -l