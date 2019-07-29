#  一.准备工作

 1.安装<a href="http://nodejs.org/">node.js </a>
 </br>
 2.安装<a href="https://git-scm.com/">Gith </a>
 </br>
 3.注册<a href="https://github.com">github</a>
# 二.配置Git对Github的操作
 1.打开Git bash，之后进行按照顺序进行命令操作
 </br>
 2.配置用户名：git config --global user.name "客户端用户名（随意填个喜欢的名字)"
 </br>
 3.配置邮箱：git config --global user.email “邮箱"
 </br>
 4.查看Git配置：git config --list
 </br>
 5.修改用户名：git config --global --replace-all user.name "输入新用户名"
 </br>
 6.修改邮箱：git config --global --replace-all user.email "输入新邮箱" 
 </br>
 7.生成SSH密钥：ssh-keygen -t rsa -C “客户端配置的邮箱”
 </br>
 8.查看密钥（复制备用）：cat ~/.ssh/id_rsa.pub
 </br>
 9.注册GitHub，点击右上方的:New repository
 </br>
 10.Repository name命名为：你的github名称.github.io
 </br>
 11.注意：不要勾选Initialize this repository with a README前面的框
 </br>
 12.之后进入新建的这个github库，点击Settings
 </br>
 13.点击Deploy keys->Add deploy keys
 </br>
 14.title随意填写,将第8步复制的内容粘贴进去
 </br>
 15.Add key
 </br>
 **此时,你已经获得了Git对Github的控制**
# 三.建立静态网站
 1.找到一个你想放文件的磁盘,并新建文件为hexo(以d盘为例)
 </br>
 2.之后打开cmd
 </br>
 3.首先输入d：(进入d盘)-->cd hexo(进入hexo文件夹下)
 </br>
 4.下载：npm install hexo-cli -g
 </br>
 5.下载文件：hexo  init blog
 </br>
 6.生成新静态页面：hexo g
 </br>
 7.查看静态页面：hexo s(你可以进行查看，如果没兴趣我们继续来往下走)
 </br>
 8.用Vscode或者其他的编译器打开你的在d盘的hexo文件下的blog文件
 </br>
 9.在这里面有个_config.yml文件，打开文件，鼠标拖动到最后，在deploy下改写
 </br>
 10.type ：git
  repo：https://github.com/你的github名字/你的github名字.github.io.git
 </br>
 11.然后Ctrl+s保存
 </br>
 12.打开你的cmd(确认操作在d盘的hexo的blog文件下)
 </br>
 13.上传你的文件至github库：hexo d
 </br>
 14.打开网页输入网站地址：https://你的github名字.github.io/ 查看你的网站
# 其他说明
<a href="https://hexo.io/zh-cn/docs/">Hexo官方文档</a>
</br>
<a href="https://space.bilibili.com/362224537/">B站视频教学</a>
</br>
请结合我的内容与这些教学视频官方文档共同查看建站,如果你有更多以问题,请
<a href="http://wpa.qq.com/msgrd?v=3&uin=603329354&site=qq&menu=yes">联系我</a>



