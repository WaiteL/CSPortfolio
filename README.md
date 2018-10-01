# csPortfolio
* WebPage [here]()
* Lightning [here](https://github.com/WaiteL/Lightning/blob/master/lighting2.pde)

```Java
int startx=0;
int starty=150;
int endx=0;
int endy=150;

void setup()
{
  strokeWeight(3);
  background(27, 2, 55);
  size(300,300);
}

void draw()
{
  stroke((int)(Math.random()*256),(int)(Math.random()*256),(int)(Math.random()*256));

  while(endx<301){

  endx = startx + (int)(Math.random() * 10) + 0;
  endy = starty + (int)(Math.random()*19)+ -9;

  line(startx,starty,endx,endy);
  startx=endx;
  starty=endy;
}
}

void mousePressed()
{
  startx=0;
  starty=150;
  endx=0;
  endy=150;

}
```
* Lightning JS [here](https://github.com/WaiteL/lightning-JS/blob/master/lightingJS.js)

``` Java Script

var startx=0;
var starty=150;
var endx=0;
var endy=150;

  function setup()
{
createCanvas(300,300);
strokeWeight(3);
background(27, 2, 55);
}
  function draw()
{
stroke((int)(Math.random()*256),(int)(Math.random()*256),(int)(Math.random()*256));

  while(endx<301){

endx = startx + (int)(Math.random()*10);
endy = starty + (int)(Math.random()*19)-9;

line(startx,starty,endx,endy);
startx=endx;
starty=endy;
}
}

function mousePressed()
{
startx=0;
starty=150;
endx=0;
endy=150;
}
```
