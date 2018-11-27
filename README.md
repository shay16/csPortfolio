# Shayla's Computer Science Portfolio
Lab | Link 
--- | --- 
*Still* | `renders` 
1 | 2 

* WebPage [here](https://shay16.github.io/testPage/swimPage/)
  > I really enjoyed making the website! I appreciated being able to design and format the website.
* Lightning [here](https://shay16.github.io/lightning2/)
  > I liked the lightning project. I had some difficulty getting the lightning to stay on the screen.
* Dice [here](https://shay16.github.io/dice3/)
  > I struggled with the dice project. It took a lot of trial and error to complete.
* Starfield [here](https://shay16.github.io/starfield5/)
  > Starfield was my favorite project. I really enjoyed designing it!
* Chemotaxis [here](https://shay16.github.io/chemotaxis4/)
  > Chemotaxis was very challenging.I struggled getting the sharks to move the way I wanted. I am very happy with the end result.
* College Presentation [here](https://docs.google.com/presentation/d/e/2PACX-1vSVdh9hhiTJKJZ2vKc1Ja0nFpV8B8eXYnVDWg5tvQ0k54pX715NL7UGem1VObwyCgV9bVhpr7UcQmYS/pub?start=false&loop=false&delayms=3000)
  > I really enjoyed this assignment. I researched the University of Illinois Urbana Champaign! I loved learning about all the university >has to offer. 
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
