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
  
## Reflection:

###Sources of pride in programming development:  
>Two things that are a source of pride in my program development are my starfield and chemotaxis projects. I enjoyed being able to incorporate design into both projects. I learned a lot about the different functions of Math.random. I am really happy with the final outcome of these two projects. The two projects are accomplishments because they both took a lot of time, effort, and learning to make but they turned out really well.  

###Most significant hurdle encountered last trimester:
>I encountered LOTS of challenges throughout the trimester. One of the most significant hurdles I encountered was getting all of the dice to roll a random number between 1 and 6 and placing the corresponding amount of dots in the correct position. I resolved this issue by starting with just one die and with a lot of trial and error I was able to get the die to roll and the dots in the correct place. After that I was able to incorporate it on all of the dice. I typically have trouble getting the projects going but once they start to function I really enjoy adding different aspects of design.  

###Challenging code:
>I struggled making the OddballParticle class. I wanted the class to rotate the opposite direction of the NormalParticle and JumboParticle classes. I ended up finding a simple solution to this issue. I was able to get it to move the opposite direction by subtracting the angle instead of adding it. Another thing I did was work with the speed of the particles so the OddballParticle class moves at a slower rate than the NormalParticle and JumboParticle classes. I worked collaboratively with Dr. R to get the original circular motion of the Particle class and I worked individually on the rest of the starfield project. 



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
