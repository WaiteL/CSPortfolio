# **csPortfolio**

## **Lightning** [*here*](https://github.com/WaiteL/Lightning/blob/master/lighting2.pde)

```
..* Java

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
```

## **Lightning JS** [*here*](https://github.com/WaiteL/lightning-JS/blob/master/lightingJS.js)

```
..* Java Script

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
```
  
  ## **chemotaxis** [*here*](https://github.com/WaiteL/chemotaxis4/blob/gh-pages/Chemotaxis.pde)
 
```
..* Java
  
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
   ## **Starfield** [*here*](https://github.com/WaiteL/starfield5/blob/gh-pages/Starfield.pde)
 
 ```
 ..* Java
 
 public class NormalParticle implements Particle {
  double x, y, speed, angle;
  NormalParticle() {
    x =width/2;
    y =height/2;
    ///what does this do?
    angle=Math.random()*Math.PI*2;
    speed=3;
  }
  public void move() {
    x+= Math.cos(angle) * speed;
    y+= Math.sin(angle) * speed;
  
    
    ///what does this do?
    angle+=.045;
    
  }
  ```
  
 ## **Airforce Presentation** [*here*](https://docs.google.com/presentation/d/1Azlu7a9b8MLRFZQx-q3OFckwEjSyRAhu1hGTPwVeKHA/edit#slide=id.p)
 
 
