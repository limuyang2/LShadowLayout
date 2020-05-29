[![](https://jitpack.io/v/limuyang2/LShadowLayout.svg)](https://jitpack.io/#limuyang2/LShadowLayout)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
# LShadowLayout
### [中文](https://github.com/limuyang2/LShadowLayout/blob/master/README_CN.md)
This control is extracted from[QMUI](https://github.com/QMUI/QMUI_Android),You can adjust the depth, area, and fillet of the control's shadow  
>Invalid shadows in Android 4.4 and below

## Preview
![](https://github.com/limuyang2/LShadowLayout/blob/master/screen/demo.gif)  

### Demo download link
[demo apk](https://www.lanzous.com/i1smf4f)

## Obtain
First add in the repositories of build.gradle :  
```gradle
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

Then add in dependencies:  
```gradle
dependencies {
        // AndroidX
	implementation 'com.github.limuyang2:LShadowLayout:1.0.5'
}
```
**if you use `Android Support`，Please use the following:**  

```gradle
dependencies {
	implementation 'com.github.limuyang2:LShadowLayout:1.0.3'
}
```

## Use
The controls already included in this library are:  
`ShadowLinearLayout`  
`ShadowRelativeLayout`  
`ShadowConstraintLayout`  
`ShadowFrameLayout`

Simply replace the corresponding layout in the project.  
E.g：  
```xml
    <top.limuyang2.shadowlayoutlib.ShadowLinearLayout
        …………
        android:background="#fff"
        android:padding="12dp"
        app:l_radius="3dp" //Rounded corner size
        app:l_shadowAlpha="0.2"  //Shadow alpha
        app:l_shadowElevation="5dp" //Shadow value >
        
    </top.limuyang2.shadowlayoutlib.ShadowLinearLayout>
```
More properties, please see the source code


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
