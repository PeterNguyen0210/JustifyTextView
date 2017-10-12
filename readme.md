# JustifyTextView
这个项目是初学开发时写的，当时因为 TextView 行尾出现参差不齐的情况纠结了好一阵，所以才想到去自定义一个 TextView

近日看到这两篇文章，才想起之前写的这个

[微信团队披露：微信界面卡死超级bug“15。。。。”的来龙去脉](https://zhuanlan.zhihu.com/p/29996576)

[能不能先把脑袋理清楚再自吹自擂——评《微信界面卡死超级bug“15。。。。”的来龙去脉》一文](https://zhuanlan.zhihu.com/p/30050183)

## 使用

#### gradle

```
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

```
dependencies {
    compile 'com.github.nyakokishi:JustifyTextView:1.0'
}
```

#### xml

```xml
<io.github.leibnik.justifytextview.JustifyTextView
        xmlns:app="http://schemas.android.com/apk/res-auto"
        app:line_space="3px"
        app:character_space="0px"
        app:align_chars="true"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="@string/test"/>
```

`app:line_space`：配置行间距

`app:character_space`：配置字符间距

`app:align_chars`：是否完全对齐字符，默认完全对齐，仅在文本包含 CJK 字符时有效

## 效果

#### 下图为居中‘硬’对齐效果23333：

![](http://ww3.sinaimg.cn/mw690/b5405c76gw1f2sa7nkghhj20de0l50w5.jpg)

#### 下图为居中‘软’对齐效果hhhhh：

![](http://ww4.sinaimg.cn/mw690/b5405c76gw1f2sa7n2s6yj20dc0l60w8.jpg)

# License

    The MIT License (MIT)

    Copyright (c) 2016 leibnik

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.