# IOSDIalogMaster
ios风格的安卓弹出框和底部弹出框
# gradle用户
如果你是gradle用户，那么使用将会很方便，但使用之前要注意一下几点：
## 1.在build.gradle(Project:xxx)中更改并添加
```gradle
 allprojects {
        repositories {
            jcenter()
            maven { url 'https://jitpack.io' }
        }
    }
```
## 2.在build.gradle(Module:app)的dependencies中添加
```gradle
compile 'com.github.string-lzc:IOSDIalogMaster:1.0'
```
## 3.由于图片格式的问题在引用该项目是会抛异常，解决方法：在build.gradle(Module:app)文件的android项下添加：
```gradle
aaptOptions {
        cruncherEnabled = false
        useNewCruncher = false
    }
```

至此，你便可以引用该远程库了。
