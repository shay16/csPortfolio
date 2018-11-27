# Shayla's Computer Science Portfolio
Lab | Link 
--- | --- 
*Still* | `renders` 
1 | 2 

* WebPage [here](https://shay16.github.io/testPage/swimPage/)
* Lightning [here](https://shay16.github.io/lightning2/)
* Dice [here](https://shay16.github.io/dice3/)
* Starfield [here](https://shay16.github.io/starfield5/)
* Chemotaxis [here](https://shay16.github.io/chemotaxis4/)
* College Presentation [here](https://docs.google.com/presentation/d/e/2PACX-1vSVdh9hhiTJKJZ2vKc1Ja0nFpV8B8eXYnVDWg5tvQ0k54pX715NL7UGem1VObwyCgV9bVhpr7UcQmYS/pub?start=false&loop=false&delayms=3000)
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
