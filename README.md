# Python Scripting Process (.gifs and selected combinations)

## Animated combinations of letters

![Letters animation Python Scripting .gif format](animated/all3.gif)

## Single Letters

<img src="animated/S8.gif" alt="Single letter animation py script" width="300" >

```python
for i in range(frames):
  factor = i / frames

  thickness = startThickness + (nextThickness-startThickness) * factor
  middleLine = startMiddleLine + (nextMiddleLine-startMiddleLine) * factor
  roundness = startRoundness + (nextRoundness-startRoundness) * factor
  propNumb = startPropNumb + (nextPropNumb-startPropNumb) * factor


  if propNumb == 0:
  propNumb = 0.000001

  newPage(glyphWidth , capHeight/4 * len(lines))
  translate(0, height()-capHeight)

  for line in lines:
      with savedState():
        for func in line:
          func()
      translate(0, -capHeight)


  startThickness = nextThickness
  startMiddleLine = nextMiddleLine
  startRoundness = nextRoundness
  startPropNumb = nextPropNumb

```

<img src="animated/gif14_b.gif" alt="Single letter animation py script" width="300" >
<img src="animated/C.gif" alt="Single letter animation py script" width="300" >



### Archive of chosen combinations

Step by step transition
![](/chosen/_1.jpg)
![](/chosen/_2.jpg)
![](/chosen/_3.jpg)
![](/chosen/_4.jpg)
![](/chosen/_5.jpg)
![](/chosen/_6.jpg)
![](/chosen/_7.jpg)
![](/chosen/_8.jpg)
![](/chosen/_9.jpg)
![](/chosen/_10.jpg)
![](/chosen/_11.jpg)
![](/chosen/_12.jpg)
![](/chosen/_13.jpg)


Mixed
![](/chosen/2.jpg)
![](/chosen/3.jpg)
![](/chosen/4.jpg)
![](/chosen/5.jpg)
![](/chosen/_0.jpg)
![](/chosen/6.jpg)
![](/chosen/7.jpg)
![](/chosen/8.jpg)
![](/chosen/9.jpg)
![](/chosen/10.jpg)
![](/chosen/11.jpg)
![](/chosen/12.jpg)
![](/chosen/13.jpg)
![](/chosen/14.jpg)
![](/chosen/15.jpg)
![](/chosen/16.jpg)
![](/chosen/17.jpg)
![](/chosen/18.jpg)
![](/chosen/19.jpg)
![](/chosen/20.jpg)
![](/chosen/21.jpg)
![](/chosen/22.jpg)
![](/chosen/23.jpg)
![](/chosen/24.jpg)
![](/chosen/25.jpg)
![](/chosen/26.jpg)
![](/chosen/twon12.jpg)

# Testing

### Test with changing the size of the page

![](animated/twonl-test-changing-pageSize.gif)


### Test with changing the width and height of the glyphs

![](animated/twonl-test-changing-glyph-width-and-height.gif)

### Presentation of the letters which don't include circular shapes. That demonstrates how it does look without letters overlapping much and without the contrast added by the way the circularly shaped latters behave.

![](animated/twon14.gif)


### One other animated combination

![](animated/twon7.gif)
