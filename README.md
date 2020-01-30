# fabric

## 正方形

```js
var rect = new fabric.Rect({
  width: 30,
  height: 30,
  left: 10,
  top: 10,
  fill: 'red'
})
```

## 圆形

```js
var circle = new fabric.Circle({
  radius: 20,
  left: 50,
  top: 20,
  fill: 'red'
})
```

## 三角形

```js
var triangle = new fabric.Triangle({
  width: 60,
  height: 40,
  left: 40,
  top: 150,
  fill: 'blue'
})
```

> 圆形

1.fabric.Circle

2.fabric.Ellipse

3.fabric.Line

4.fabric.Polygon

5.fabric.Polyline

> 正方形

6.fabric.Rect

> 三角形

7.fabric.Triangle

```
可以简单的使用set来控制对象属性
positioning — left, top;
dimension — width, height;
rendering — fill, opacity, stroke, strokeWidth;
scaling and rotation — scaleX, scaleY, angle;
and even those related to flipping — flipX, flipY.
```

## Image（图片）

```js
let canvas = new fabric.Canvas('canvas')
fabric.Image.fromURL('./loading.jpg', oImg => {
  oImg.scale(0.5)
  canvas.add(oImg)
})
```

## path

```js
let canvas = new fabric.Canvas('canvas')
var path = new fabric.Path('M 0 0 L 200 200 L 300 200 z')
path.set({
  fill: 'red',
  stroke: 'black',
  opacity: 0.8,
  left: 100,
  top: 50
})
```
