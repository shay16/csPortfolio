# csPortfolio


* WebPage [here](https://shay16.github.io/testPage/swimPage/)
* Lightning [here](https://shay16.github.io/lightning2/)
* Dice [Here](https://shay16.github.io/Dice3/)
* Starfield [here](https://shay16.github.io/starfield5/)
* Chemotaxis [here](https://shay16.github.io/chemotaxis4/)
```Java
void draw()
{
  background(0);
  photo.resize(0, 200);
  image(photo, 50, 90);
  while (endX<400) {
    endX =startX +(int)(Math.random()*9);
    endY =startY +(int)(Math.random()*19)-9;
    line(startX, startY, endX, endY);
    startX=endX;
    startY=endY;
    println("startX" +startX);
    println("startY" +startY);
  }
}
```
