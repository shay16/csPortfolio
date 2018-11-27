# Shayla's Computer Science Portfolio

* WebPage [here](https://shay16.github.io/testPage/swimPage/)
  > I really enjoyed making the website! I appreciated being able to design and format the website.
* Lightning [here](https://shay16.github.io/lightning2/)
  > I liked the lightning project. I had some difficulty getting the lightning to stay on the screen.
* Dice [here](https://shay16.github.io/dice3/)
  > I struggled with the dice project. It took a lot of trial and error to complete.
* Starfield [here](https://shay16.github.io/starfield5/)
  > Starfield was my favorite project. I really enjoyed designing it!
* Chemotaxis [here](https://shay16.github.io/chemotaxis4/)
  > Chemotaxis was very challenging. I struggled getting the sharks to move the way I wanted. I am very happy with the end result.
* College Presentation [here](https://docs.google.com/presentation/d/e/2PACX-1vSVdh9hhiTJKJZ2vKc1Ja0nFpV8B8eXYnVDWg5tvQ0k54pX715NL7UGem1VObwyCgV9bVhpr7UcQmYS/pub?start=false&loop=false&delayms=3000)
  > I really enjoyed this assignment. I researched the University of Illinois Urbana Champaign! I loved learning about all the university has to offer. 
  
Questions:

What is one or two things that are a source of pride in your programming development?  
>
Identify the most significant hurdle you encountered last trimester.  Write about what it was and how it was resolved.
>
Chalenging code:

```Java
class OddballParticle implements Particle {
  double x, y, speed, angle;
  OddballParticle() {
    x=width/2;
    y=height/2;
    speed=Math.random()*4;
    angle=(Math.random())*Math.PI*2;
  }
  void move() {
    x+=Math.cos(angle)*speed;
    y+=Math.sin(angle)*speed;
    angle-=.020;
  }
  void show() {
    fill(255);
    //fill(((int)Math.random()*205+50), ((int)Math.random()*205+50), ((int)Math.random()*205+100));
    ellipse((int)x, (int)y, 10, 10);
  }
}
```
