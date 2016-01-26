**在Android Studio中导入SlidingMenu**

参考了好多网上文章的方法，自己也做个记录。

1.  在GitHub上下载SlidingMenu [https://github.com/jfeinstein10/SlidingMenu](https://github.com/jfeinstein10/SlidingMenu)

2.  在AS项目中新建文件夹，如明明为：library，与app文件夹同级别

3.  在settings.gradle文件中添加 include ":sliding_menu'

4.  在build.gradle(Module:app)中添加依赖

     dependencies {

     compile fileTree(include: ['*.jar'], dir: 'libs')

     compile 'com.android.support:appcompat-v7:21.0.2'

     compile project(':sliding_menu')

}

1.  修改错误：修改 library中的 build.gradle

     android {

     compileSdkVersion 22

     buildToolsVersion "22.0.1"

     与 app中的 build.gradle中的相同

     修改library中的 build.gradle

     dependencies {

         <span class="hljs-keyword">classpath</span> <span class="hljs-string">'com.android.tools.build:gradle:2.0.0-alpha5'</span>

 }

     与 build.gradle中的相同

2.  Build/Make Project 没有错误证明已经成功了