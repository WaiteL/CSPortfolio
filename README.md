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
* Die [here](https://github.com/WaiteL/dice3/blob/gh-pages/dieJava.pde)
``` Java

void setup()
{
  size(830, 830);
  background(30, 30, 30);
  noLoop();
}
void draw()
{
  int xpos=-50;
  int ypos=-50;
  for (int i=0; i< 15; i++) {
    ypos=ypos+=55;
   xpos=-50;
  for (int t=0; t<15; t++){
      xpos=xpos+=55;
    Die die=new Die(xpos,ypos);
    fill(30,30,30);
    stroke(0,255,0);
    rect(xpos, ypos, 50, 50,10);
    die.roll();
  }
  }
  
  
}
void mousePressed()
{
  redraw();
}
class Die //models one single dice cube
{
  int count=0;
  int x;
  int y;
  Die(int x, int y) //constructor
  {
   this.x=x;
   this.y=y;
  }
  void roll()
  {
   
  count=(int)(Math.random()*6)+1;
   
    if (count==1){
    fill(0,255,0);
      textSize(50);
      text("1", x+10,y+43);
      
    }
      if (count==2){
        fill(0,255,0);
        textSize(50);
      text("2", x+10,y+43);
        
    }
    if (count==3){
        fill(0,255,0);
      textSize(50);
      text("3", x+10,y+43);
      
    }
    if (count==4){
        fill(0,255,0);
      textSize(50);
      text("4", x+10,y+43);
      
    }
    if (count==5){
      fill(0,255,0);
       textSize(50);
      text("5", x+10,y+43);
    }
    if (count==6){
      fill(0,255,0);
      textSize(50);
      text("6", x+10,y+43);
      
    }
    
  }
  void show()
  {
    textSize(100);
    text("total is: "+count,200,800);
     ```
  
  * chemotaxis [here](https://github.com/ACS-Curriculum/chemotaxis4/blob/gh-pages/Chemotaxis.pde)
 
 ``` Java
   void follow(){

    int xdiff=x-mouseX;
    int ydiff=y-mouseY;

    float angle=0;
 
    if (xdiff==0) {
      if (ydiff<0) {
        angle=PI/2;
      } else if (ydiff>0) {
        angle=PI*1.5;
      } else {
        return;
      }
    }
       if(xdiff==0&&ydiff==0){
      ellipse (mouseX, mouseY, 10, 10);
     return;
    }
    if (xdiff!=0) {
      angle = atan(ydiff/xdiff);
    }
    ```
  }
}
```
