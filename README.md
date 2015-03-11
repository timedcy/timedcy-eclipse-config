# 下载最新合适版本的eclipse
修改配置文件eclipse.ini

-vm
D:\Program Files\Java\jdk1.7.0_25\bin\javaw.exe
-startup
plugins/org.eclipse.equinox.launcher_1.3.0.v20140415-2008.jar
--launcher.library
plugins/org.eclipse.equinox.launcher.win32.win32.x86_64_1.1.200.v20140603-1326
-product
org.eclipse.epp.package.jee.product
--launcher.defaultAction
openFile
--launcher.XXMaxPermSize
512M
-showsplash
org.eclipse.platform
--launcher.XXMaxPermSize
512m
--launcher.defaultAction
openFile
--launcher.appendVmargs
-vmargs
-Dosgi.requiredJavaVersion=1.7
-Xms512m
-Xmx1724m
-XX:+UseParallelGC
-XX:PermSize=456M
-XX:MaxPermSize=512M


# 添加jre7
在installed jre中添加jdk7，否则可能不能正常配置Pydev


#安装插件
从Help --> Eclipse Marketplace安装
Eclipse Moonrise UI Theme
Pydev
Maven Integration
JadEclipse


# 配置和偏好设置
增加local history备份数
文件编码改为UTF8
设置Dark ui
java --> code style --> formatter下导入代码格式配置timedcy-java-codestyle-formatter.xml，则可以自动格式化
java --> code style --> Templates下导入代码模板配置timedcy-java-codestyle-templates.xml，则可以套用注释模板
java --> editor --> Templates下导入编辑模板配置timedcy-java-editor-templates.xml，则可以用sb/newmap/formap/logger/logi/loge/strf等快捷键
General --> Keys --> Content Assist设置Ctrl+Space为快捷键唤出自动提示
配置python路径、maven路径

