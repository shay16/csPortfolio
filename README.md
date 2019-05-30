# Shayla's Computer Science Portfolio!

* WebPage [here](https://shay16.github.io/testPage/swimPage/)
  > I really enjoyed making the website! I appreciated being able to design and format the website.
* Dice [here](https://shay16.github.io/dice3/)
  > I struggled with the dice project. It took a lot of trial and error to complete.
* Starfield [here](https://shay16.github.io/starfield5/)
  > Starfield was a fun project. I really enjoyed designing it!
* Chemotaxis [here](https://github.com/shay16/Chemo/blob/master/Screenshot%20(15).png)
  > Chemotaxis was very challenging. I struggled getting the sharks to move the way I wanted. I am very happy with the end result.
* College Presentation [here](https://docs.google.com/presentation/d/e/2PACX-1vSVdh9hhiTJKJZ2vKc1Ja0nFpV8B8eXYnVDWg5tvQ0k54pX715NL7UGem1VObwyCgV9bVhpr7UcQmYS/pub?start=false&loop=false&delayms=3000)
  > I really enjoyed this assignment. I researched the University of Illinois Urbana Champaign! I loved learning about all the university has to offer. 
* Holiday Card [here](https://github.com/shay16/Holiday-Card.git)
 
## Reflection:
### Favorite Projects:
>Bachelor Projects
<details>
<summary>Bachelor Map</summary>
<br>
  
  ![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(10).png "Logo Title Text 1")
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(9).png "Logo Title Text 1")

  ### Difficulties or opportunities you encountered along the way.

The toughest part was...

### Most interesting piece of your code and explanation for what it does.

```Java
void keyPressed() {
if (keyCode == LEFT) {
   tree= tree.getLeft();
   System.out.println(tree.getValue());
   String s=(String)tree.getValue();
   fill(155);
   textSize(50);
} else if (keyCode == RIGHT) {
   tree = tree.getRight();
   System.out.println(tree.getValue());
   String s=(String)tree.getValue();
   fill(155);
   textSize(50);
} else if (tree.getLeft()==null&&tree.getRight()==null) {
   System.out.println(tree.getValue());
   tree=t.returnTree();
}
}
```
This is the code that moves down the tree as decisions are made. It gets each value from both left and right and also casts the value to a String. If the progressions arrives at the leaf nodes, those values are printed.
## Built With

* [Processing](https://processing.org/) - The IDE used

## Authors

* **Shayla**
* **Sydney**
* **Madison**


## Acknowledgments

* Dr. R.
* The Bachelor
</details>

![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(10).png "Logo Title Text 1")
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(9).png "Logo Title Text 1")
<details>
  
<summary>Bachelor Tree</summary>

<br>

![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(16).png "Logo Title Text 1")
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(17).png "Logo Title Text 1")


</details>

### Sources of pride in programming development:  
>Two things that are a source of pride in my program development are my starfield and chemotaxis projects. I enjoyed being able to incorporate design into both projects. I learned a lot about the different functions of Math.random. I am really happy with the final outcome of these two projects. The two projects are accomplishments because they both took a lot of time, effort, and learning to make but they turned out really well.  

### Most significant hurdle encountered last trimester:
>I encountered LOTS of challenges throughout the trimester. One of the most significant hurdles I encountered was getting all of the dice to roll a random number between 1 and 6 and placing the corresponding amount of dots in the correct position. I resolved this issue by starting with just one die and with a lot of trial and error I was able to get the die to roll and the dots in the correct place. After that I was able to incorporate it on all of the dice. I typically have trouble getting the projects going but once they start to function I really enjoy adding different aspects of design.  

### Challenging code:
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

