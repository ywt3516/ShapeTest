# ShapeTest


>在drawable文件夹下创建Drawable resource file文件.xml
可以再TextView/LinearLayout/Button等控件添加android:background="@drawable/tv_test3"
用于改变其形状。

## 1.标签shape
```
      shape 形状
        android:shape=["rectangle" | "oval" | "line" | "ring"]  
        shape的形状，默认为矩形，可以设置为矩形（rectangle）、椭圆形(oval)、线性形状(line)、环形(ring)
        当android:shape="ring"时：
        android:innerRadius       尺寸，内环的半径。
        android:innerRadiusRatio  浮点型，以环的宽度比率来表示内环的半径。
        例如:
            如果android:innerRadiusRatio，表示内环半径等于环的宽度                
            除以5，这个值是可以被覆盖的，默认为9.
         android:thickness           尺寸，环的厚度
         android:thicknessRatio      浮点型，以环的宽度比率来表示环 
         的厚度，例如，如果android:thicknessRatio="2"，
         那么环的厚度就等于环的宽度除以2。这个值是可以被 
         android:thickness覆盖的，默认值是3.
         android:useLevel            boolean值，如果当做是      
         LevelListDrawable使用时值为true，否则为false.
```
## 2.标签solid
```
    solid  内部填充
    <solid android:color="#F5F5F5" />
    表示填充内部颜色
```    
## 3.标签corners
```
    corners  圆角
    <corners android:radius="5dp" />
    android:radius              整型 半径   圆角的半径 值越大角越圆
    <corners
        android:bottomLeftRadius="5dp"
        android:bottomRightRadius="5dp"
        android:topLeftRadius="5dp"
        android:topRightRadius="5dp" />
    android:topLeftRadius       整型 左上角半径
    android:topRightRadius      整型 右上角半径
    android:bottomLeftRadius    整型 左下角半径
    android:bottomRightRadius   整型 右下角半径
```
## 4.标签stroke
```
    stroke   边框
    <stroke
        android:width="0.01dp"
        android:color="#8e8e8e"
        android:dashGap="10dp"
        android:dashWidth="5dp"/>
    android:width       整型  描边的宽度
    android:color       颜色值     描边的颜色
    android:dashWidth   整型  表示描边的样式是虚线的宽度， 值为0
    时，表示为实线。值大于0则为虚线
    android:dashGap     整型  表示描边为虚线时，虚线之间的间隔.
```
## 5.标签size
```
    size 大小
    <size
        android:width="5dp"
        android:height="5dp" />
    android:width   整型 宽度
    android:height  整型 高度
```
## 6.标签padding
```
    padding         内边距，即内容与边的距离
    android:left    整型 左内边距
    android:top     整型 上内边距
    android:right   整型 右内边距
    android:bottom  整型 下内边距
```
## 7.标签gradient 
```
gradient  渐变色
    android:startColor  颜色值          起始颜色
    android:endColor    颜色值          结束颜色
    android:centerColor 整型            渐变中间颜色，即开始颜色与结束颜色之间的颜色
    android:angle       整型            渐变角度(PS：当angle=0时，渐变色是从左向右。 然后逆时针方向转，当angle=90时为从下往上。
                                        angle必须为45的整数倍)
    android:type          ["linear" | "radial" | "sweep"] 渐变类型(取值：linear、radial、sweep)
                          linear 线性渐变，这是默认设置
                          radial 放射性渐变，以开始色为中心。
                          sweep 扫描线式的渐变。
   android:useLevel       ["true" | "false"] 如果要使用LevelListDrawable对象，就要设置为true。设置为true无渐变。false有渐变色
   android:gradientRadius 整型            渐变色半径.当 android:type="radial" 时才使用。单独使用 android:type="radial"会报错。
   android:centerX        整型            渐变中心X点坐标的相对位置
   android:centerY        整型            渐变中心Y点坐标的相对位置
```
    









      
