# three.js 创建简单场景

##主要使用的three基础几何形状

CylinderGeometry 柱体类

```
THREE.CylinderGeometry(radiusTop, radiusBottom, height, radiusSegments, heightSegments, openEnded)

```
 radiusTop 与 radiusBottom 分别是顶面和底面的半径，由此可知，当这两个参数设置为不同的值时，实际上创建的是一个圆台； height 是圆柱体的高度； radiusSegments 与 heightSegments 可类比球体中的分段； openEnded 是一个布尔值，表示是否没有顶面和底面，缺省值为false，表示有顶面和底面



SphereGeometry 是球体类

```
THREE.SphereGeometry(radius, segmentsWidth, segmentsHeight, phiStart, phiLength, thetaStart, thetaLength)

```
radius 是半径； segmentsWidth 表示经度上的切片数； segmentsHeight 表示纬度上的切片数； phiStart 表示经度开始的弧度； phiLength 表示经度跨过的弧度； thetaStart 表示纬度开始的弧度； thetaLength 表示纬度跨过的弧度), 其中需要注意的是在使用时可以根据经纬度切片数来定制球形外形, 可以通过经纬度弧度来定制球形起始形状



 用CylinderGeometry、SphereGeometry 创建花朵，以及基本的树枝。主要用到了旋转、缩放和平移。由于要注意创建的柱状体的组合，需要计算在x、y、z方向的平移位置。



##效果

![](https://img-blog.csdn.net/20180119142734733?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvY2NfZnlz/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)



