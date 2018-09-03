[![](https://jitpack.io/v/limuyang2/LShadowLayout.svg)](https://jitpack.io/#limuyang2/LShadowLayout)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
# LShadowLayout
本控件提取自[QMUI](https://github.com/QMUI/QMUI_Android)，可以调整控件阴影的 深浅、面积、以及圆角  

## 预览
![](https://github.com/limuyang2/LShadowLayout/blob/master/screen/demo.gif)  

### demo下载地址
[demo apk](https://www.lanzous.com/i1smf4f)

## 获取
先在 build.gradle 的 repositories 添加：  
```gradle
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

再在dependencies添加：  
```gradle
dependencies {
	implementation 'com.github.limuyang2:LShadowLayout:1.0'
}
```

## 使用
本库中已包含的控件有：  
```ShadowLinearLayout```线性布局  
```ShadowRelativeLayout```相对布局  
```ShadowConstraintLayout```约束布局  
仅需替换项目中对应的布局即可。  
例如：  
```xml
    <top.limuyang2.shadowlayoutlib.ShadowLinearLayout
        …………
        android:background="#fff"
        android:padding="12dp"
        app:l_radius="3dp" //圆角大小
        app:l_shadowAlpha="0.2"  //阴影值
        app:l_shadowElevation="5dp" //Z轴高度 >
        
    </top.limuyang2.shadowlayoutlib.ShadowLinearLayout>
```
更多属性请查看源码


## License
```
2018 limuyang
Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
