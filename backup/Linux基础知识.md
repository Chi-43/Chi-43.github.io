# Linux学习

## 1 工具
### 1.1 使用MobaXterm连接Linux
<img width="1232" height="845" alt="Image" src="https://github.com/user-attachments/assets/0607b410-8efa-4eb2-bb96-a4d4548f04c3" />

### 1.2 vim编辑器
<img width="1036" height="446" alt="Image" src="https://github.com/user-attachments/assets/3eab609f-c43c-4dd4-a2ad-39ec6534b3ae" />

vim 文件路径
如果文件路径不存在 则创建文件
vim hello.txt //进入命令模式
按键盘**i**，进入输入模式
在输入模式内输入内容
输入完成后，按**esc**回退回命令模式
在命令模式内 按键盘:进入底线命令模式
在底线命令内输入 **:wq** 保存文件并退出vim编辑器

## 2 linux 基础命令
### 2.1 Linux的目录结构
<img width="1147" height="357" alt="Image" src="https://github.com/user-attachments/assets/73e7fd07-4a5b-4740-9a3e-d07c6d16ad69" />

Window使用\ Linux使用/

<img width="968" height="288" alt="Image" src="https://github.com/user-attachments/assets/f8274301-41c5-46b1-b152-32c630fbb771" />

- cd /test/hello.txt
- cd /itheima.txt
- cd /itcast/itheima/hello.txt

## 2.2 Linux命令基础
<img width="742" height="550" alt="Image" src="https://github.com/user-attachments/assets/5f9da6e3-6d9d-4028-86d2-c71033aaa23b" />

### 2.2.1 ls命令
<img width="854" height="285" alt="Image" src="https://github.com/user-attachments/assets/62edf587-b207-42eb-b6b0-ff7df0b6a761" />
- -a选项 表示all的意思 即列出所有文件 包括隐藏的文件
- -l选项 表示以列表的形式展示内容，并展示更多的信息
- -h选项 需要和-l选项搭配使用，以更人性化的方式展示文件的大小单位
- ls -lah 等价于 ls -l -a -h

### 2.2.2 特殊路径符
<img width="873" height="127" alt="Image" src="https://github.com/user-attachments/assets/b6d8650a-fc28-4e02-ac48-e48f12516349" />

### 2.2.3 mkdir
<img width="1606" height="409" alt="Image" src="https://github.com/user-attachments/assets/10aeac8e-c9e6-4062-b5e2-b159f68397d1" />
<img width="1347" height="536" alt="Image" src="https://github.com/user-attachments/assets/c3f154f4-933f-4b7a-8ed0-809b7cfe8055" />

eg. mkdir -p chi/chi1/nice/666

### 2.2.4 touch创建文件
<img width="1839" height="540" alt="Image" src="https://github.com/user-attachments/assets/37bcf3f8-d5de-47dc-8d72-9a194d13d3f1" />

### 2.2.5 cat查看文件
 语法： cat Linux路径

### 2.2.6 more命令查看文件内容
<img width="782" height="211" alt="Image" src="https://github.com/user-attachments/assets/3124eee8-f89d-4823-bcec-cc3ab9520871" />

more 按空格翻页   按q退出

### 2.2.7 cp命令复制文件文件夹
<img width="529" height="171" alt="Image" src="https://github.com/user-attachments/assets/1baba133-05ff-42ee-895b-048d77996118" />

### 2.2.8 mv命令移动文件文件夹
<img width="1738" height="329" alt="Image" src="https://github.com/user-attachments/assets/1bdadaf5-81d9-4d4d-8438-c6fde1430fdd" />

mv命令还可实现文件改名的效果 eg mv test1.txt test2.txt

### 2.2.9 rm删除文件文件夹
<img width="598" height="240" alt="Image" src="https://github.com/user-attachments/assets/bef333d4-7417-44c7-802f-cd7770811913" />

<img width="649" height="240" alt="Image" src="https://github.com/user-attachments/assets/4c6671da-b1dc-484f-b6a1-2de23397a8ce" />
<img width="512" height="84" alt="Image" src="https://github.com/user-attachments/assets/5b63df14-52b1-4ef6-8efa-a19ef5af5f49" />

### 2.2.10 which 查找命令文件(只支持命令文件的查找)
<img width="595" height="158" alt="Image" src="https://github.com/user-attachments/assets/5aa8a1c2-3011-47d5-88e9-9e74d7ae97d4" />
eg which cd  which pwd  which ls

### 2.2.11 find命令 -按文件名查找文件
可先切换到管理员权限下进行全文件的查找
<img width="489" height="67" alt="Image" src="https://github.com/user-attachments/assets/323e651b-8470-4afc-b1d2-22cbf8644d32" />
<img width="442" height="238" alt="Image" src="https://github.com/user-attachments/assets/ea8bc30d-22b7-4d26-a7db-111c80a7d42a" />

### 2.2.12 find命令 -按文件大小查找文件
<img width="504" height="306" alt="Image" src="https://github.com/user-attachments/assets/dddcdd70-abf2-4d59-977d-96ea653ec7a0" />

### 2.2.13 切换到root用户
su - root 切换到root用户
exit 回退到普通用户

### 2.2.14 grep命令(可作为管道符的内容输入端口)
<img width="792" height="170" alt="Image" src="https://github.com/user-attachments/assets/3eff3a3e-9695-4f41-81f8-b5c3ec3dbc78" />

### 2.2.15 wc命令做数量统计
<img width="442" height="242" alt="Image" src="https://github.com/user-attachments/assets/654e4968-a8bf-4fd9-ac50-ae80ec7d6dbc" />

### 2.2.16 管道符 |
将管道符左边命令的结果，作为右边命令的输入

### 2.2.17 echo命令输出指定内容
<img width="722" height="171" alt="Image" src="https://github.com/user-attachments/assets/308a747c-8e92-4ab2-a90b-d8f207cd1748" />

### 2.2.18 反引号`
被反引号(`*`)包含的内容会被作为命令执行，而非普通字符

### 2.2.19 重定向符
<img width="598" height="138" alt="Image" src="https://github.com/user-attachments/assets/b87a120f-4163-4826-b0fd-800ee95cad50" />

### 2.2.20 tail命令
<img width="709" height="206" alt="Image" src="https://github.com/user-attachments/assets/e07e3064-d337-48eb-b7e4-e4002c274939" />

## 3 用户管理权限
### 3.1 su和exit命令
<img width="1263" height="624" alt="Image" src="https://github.com/user-attachments/assets/0dbe7f55-d472-4d1c-9e0c-5800fc7247b2" />

### 3.2 sudo命令
<img width="775" height="380" alt="Image" src="https://github.com/user-attachments/assets/51d431b4-dd97-4b28-8d26-8e8bb53fe53b" />

### 3.3 为普通用户配置sudo认证
<img width="775" height="380" alt="Image" src="https://github.com/user-attachments/assets/c11fac20-d76f-46da-9c52-c58ad616de8a" />

### 3.4 用户和用户组
均需要在root命令下进行
创建用户组 groupadd 用户组名
删除用户组 groupdel 用户组名
<img width="2161" height="961" alt="Image" src="https://github.com/user-attachments/assets/94b145bd-16e6-4d4a-90f6-1d9830ecb65f" />
<img width="476" height="145" alt="Image" src="https://github.com/user-attachments/assets/5a2d80ee-c3b4-4c8f-919d-542bebc377f2" />

### 3.5权限信息
<img width="559" height="423" alt="Image" src="https://github.com/user-attachments/assets/4a44c54d-5200-487e-bf60-12d99d4a5309" />
<img width="818" height="260" alt="Image" src="https://github.com/user-attachments/assets/bc35fbfb-f532-4b7f-9143-da5ab0c16e16" />

#### 3.5.1 rwx命令信息
<img width="567" height="378" alt="Image" src="https://github.com/user-attachments/assets/a9710eef-6233-4d12-b25d-7fc0dd035884" />

### 3.6 chmod命令
<img width="1027" height="329" alt="Image" src="https://github.com/user-attachments/assets/c173eca6-8da0-4526-ac22-566432a28b92" />
<img width="700" height="117" alt="Image" src="https://github.com/user-attachments/assets/f94f7be3-6434-43ab-aed8-012c4670f35b" />

### 3.7 权限的数字序号
<img width="977" height="427" alt="Image" src="https://github.com/user-attachments/assets/e4508731-e7b8-4b3b-98dd-838bcec4f4f6" />

### 3.8 chown命令
<img width="833" height="249" alt="Image" src="https://github.com/user-attachments/assets/344819e5-b221-4a54-9cb6-63417640fcf7" />

