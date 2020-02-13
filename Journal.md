#This is the journal to Computer Science!

1. What did I do today?
For today's class, we wrote algorithm, a step-by-step directions for Dr. R to eat a sandwich. 
2. What did I learn?
I learned the importance of clear and specific directions but it was also interesting to see the compitational thinking such as finding the pattern in this activity.
3. Any questions??
I don't have any questions yet, but I am excited to learn more!

#Second Computer Science Class!

1. What did I do today?
We programmed a dice on Sketch and tested it out, as well as playing a game where we made an  unfair dice.

Below is the Program of the dice:

```.py
def setup():
    size (600,600)
    
def draw():
    x=0
    
def mouseClicked():
    background(255)
    stroke(0)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)

    
    
    n=random(0,3.1)
    print(n)
    if 0<=n<0.5:
        circle(300,300,50)
    if 0.5<=n<1.0:
        circle(200,200,50)
        circle(400,400,50)
    if 1.0<=n<1.5:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
    if 1.5<=n<2.0:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
    if 2.0<=n<2.5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
    if 2.5<=n<3.1:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
```

2. What did I learn today?

I realized the pattern and the importance of it and although it was difficult, I enjoyed seeing the program work.

3. Any questions?

How do people manage to make apps??

#Third Computer Science Class

Below is the Program of a Dice with Graphs and Automatic:

```.py

# These variables are to count the rools of the dice

2022.2.13

ones=0
twos=0
threes=0
fours=0
fives=0
sixes=0


def setup():
    size (600,600)
    background(255)
    barGraph()

def draw():
    x=0
    delay(10)
    mouseClick()
    barGraph()

def barGraph():
    global ones
    fill(0)
    textSize(20)
    for x in range (6):
        text(x+1,(50+50*x), 580) 
    strokeWeight(10)
    rect(50,550-ones, 15, ones)
    rect(100,550-twos, 15, twos)
    rect(150,550-threes, 15, threes)
    rect(200,550-fours, 15, fours)
    rect(250,550-fives, 15, fives)
    rect(300,550-sixes, 15, sixes)

   
    

def mouseClick(): 
    global ones, twos, threes, fours, fives, sixes
    background(255) 
    stroke(0) 
    fill(255)
    rect(100,100, 400, 400, 10) 
    stroke(255,0,0) 
    strokeWeight(10)

    n=random(0,6)
    print(n)
    if 0<=n<1:
        circle(300,300,50)
        ones=ones+1
        print("Number of times one has been rolled:", ones)
    if 1<=n<2:
        circle(200,200,50)
        circle(400,400,50)
        twos=twos+1
        print("Number of times  two has been rolled:", twos)
    if 2<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        threes=threes+1
        print("Number of times three has been rolled:", threes)
    if 3<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        fours=fours+1
        print("Number of times four has been rolled:", fours)
    if 4<=n<5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
        fives=fives+1
        print("Number of times five has been rolled:", fives)
    if 5<=n<6:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
        sixes=sixes+1
        print("Number of times six has been rolled", sixes
        
```
        
1. What did I do today?
I made a code on Processing of a dice that rolls on its' own and draws a graph of the number of the times each number came out.
2. What did I learn today?
The thing I remeber the most was that in order to add a graph, you can type in "print", and that each time I want to change the graph, I have to change each number inside the brakets.
3. Questions:
How do I get better?
