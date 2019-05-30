# Shayla's Computer Science Portfolio!

* WebPage [here](https://shay16.github.io/testPage/swimPage/)
  > I really enjoyed making the website! I appreciated being able to design and format the website.
* Dice [here](https://shay16.github.io/dice3/)
  > I struggled with the dice project. It took a lot of trial and error to complete.
* Starfield [here](https://shay16.github.io/starfield5/)
  > Starfield was a fun project. I really enjoyed designing it!
* Chemotaxis [here](https://github.com/shay16/Chemo/blob/master/Screenshot%20(15).png)
  > Chemotaxis was very challenging. I struggled getting the sharks to move the way I wanted. I am very happy with the end result.
* Holiday Card [here](https://github.com/shay16/Holiday-Card.git)
 

## Favorite Projects:
>Bachelor Projects
<details>
<summary>Bachelor Map</summary>
<br>
  
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(10).png "Logo Title Text 1")
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(9).png "Logo Title Text 1")

  ### Difficulties 

The toughest part was making the method that sorted through the data to find out the probability that a contestant won both the first impression rose and the final rose. This was difficult because we had to determine how to loop through the map and use the map methods to attain the information we wanted. We solved them by trial and error along with asking Dr. R. The reference sheet with map methods was also useful. Another challenge we faced was that when we were parsing through the data our program was picking up information that is wasn't supposed to which altered our counter. The inaccurate counter messed up a percentage that was crucial to the success of our project. We tackled this obstacle by taking a different approach. Instead of using the .equals method for the entire string that represented a contestant, we went through each ‘box’ of data one by one by using an array list. This solved our issue and calculated accurate percentages.


### Most interesting piece of code 

```Java
public BB(String line){
    String[] person= line.split(",");
    
    season = person[1];
    name = person[2];
    
    if(line.contains("R1"))
    R1=true;
    else
    R1=false;
    if(line.contains("W"))
    W=true;
    else
    W=false;
    
   // for(int i = 0;i<person.length;i++){
     // out.println(person[i]);
    if(line.contains(",EF,"))
      EF = true;
    else
      EF = false;
    
  }
```
This is the code that determines if the contestant received the first impression rose and the final rose.  

## Built With

* [Processing](https://processing.org/) 

## Authors

* **Shayla**
* **Sydney**
* **Madison**


## Acknowledgments

* Dr. R.
* The Bachelor
</details>

<details>
  
<summary>Bachelor Tree</summary>

<br>

![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(16).png "Logo Title Text 1")
![alt text](https://github.com/shay16/testPage/blob/gh-pages/Screenshot%20(17).png "Logo Title Text 1")

 ### Difficulties 

We encountered several difficulties. One of the challenges we faced was traversing through the tree. We keep getting a null pointer error. Another challenge we faced was when we used the mouse pressed buttons we would always end up at the last slide. We resolved the issue by changing the values of the isBetween method so it would only be called the correct number of times. We used a lot of trial and error and we eventually resolved both issues. 


### Most interesting piece of code 

```Java
TreeNode buildTree(){
     
    root = new TreeNode("Do you fall in love quickly?");
    //level one
    root.setLeft(new TreeNode("Do you like to stir the pot"));
    root.setRight(new TreeNode("What if they're Instagram famous?"));
    //level two
    root.getLeft().setRight(new TreeNode("The Bachelor" ));
    root.getRight().setLeft(new TreeNode("The Bachelorette" ));
    root.getLeft().setLeft(new TreeNode("Bachelor in Paradise" ));
    root.getRight().setRight(new TreeNode("Avoid these shows at all costs"));
  
     current = root;
     return current;
  }
```
This is the code that builds the bachelor tree
## Built With

* [Processing](https://processing.org/) 

## Authors

* **Shayla**
* **Sydney**
* **Madison**


## Acknowledgments

* Dr. R.
* The Bachelor

</details>


## Reflection

<details>
<summary>HERE</summary>
<br>

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
</details>
