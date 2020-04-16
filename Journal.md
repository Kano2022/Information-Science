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


# Online Computer Science 1

In this class, I learnt how to represent the movement of people using a circle with a random movement.
The task was to learn how to repeat the steps for ten circles without having to write it manually.
From this class, I learnt that append means to "add on" to the end of the list, and in this case, it allowed me to make all ten circles randomly move without having to type them one by one.
I still am not super sure how to use the append and loop but I think I got a bit of a hang.


```.py

#definitions of variables
x = []
y = []

def setup():
    size(500,500)
    for i in range(10):
          x.append(random(0,500))
          y.append(random(0,500))
        
def draw():
    background(255)
    strokeWeight(2)
    global x, y
    
    #FirstIndivisual
    for i in range(10):
        circle(x[i],y[i],40)
        x[i] = x[i] + random(-10,10)
        y[i] = y[i] + random(-10,10)
        
        if x[i] > 500:
            x[i] = 500
        if x[i] < 0:
            x[i] = 0
        if y[i] > 500:
            y[i] = 500
        if y[i] < 0:
            y[i] = 0
            
    delay(100)
    

```

# Online Class No.2 

In this session, I followed the video and tried to colour code the infected population to further visualize the spread of this desiease.
This was done by calculating the distance between two people (circles) first by using the Pythagorean theorem and setting each distance using the a, b, and c method.
I have many questions regarding this process, and in the end, my program did not work but I will see what the problem is later on in my meetings. Some questions are within the program by using the # mark.

```.py
#definitions of variables
x = []
y = []
h = [False, True] 

def setup():
    size(500,500)
    for i in range(10):
          x.append(random(0,500))
          y.append(random(0,500))
          h.append(True) 
    #Shouldn't the append here be random??
          
def distance(x1, x2, y1, y2):
    a = (x1 - x2)
    b = (y1 - y2)
    c = sqrt (a**2 + b**2)
    return c
        
def draw():
    background(255)
    strokeWeight(2)
    global x, y
    
    for ind in range(len(x)):
        if h[ind] == True:
            fill(255)
        else:
            fill (255, 0, 0)
    circle(x[ind], y[ind], 40)
    for nei in range(len(x)):
        if nei == ind:
            continue 
        d = distance(x[ind], x[nei], y[ind], y[nei])
    #What does this mean
        if d < 40 and (h[nei] == False or h[ind] == False):
            h[ind] = False
            h[nei] = False 
    
    #FirstIndivisual
    for i in range(10):
        circle(x[i],y[i],40)
        x[i] = x[i] + random(-10,10)
        y[i] = y[i] + random(-10,10)
        
        if x[i] > 500:
            x[i] = 500
        if x[i] < 0:
            x[i] = 0
        if y[i] > 500:
            y[i] = 500
        if y[i] < 0:
            y[i] = 0
            
     
    delay(100)
    

```

# Online Classes 2 
In this class, I practiced the "loop" by repeating multiple similar values.
Below is the program with some questions.
I learnt some simple patterns;
"for _ (any word or value) in range (__ the number you want to start, __ the number you want to end, __ By how much you want to increase):"
When putting in vocabularies, you must
for i in range:
    print ("_{0 for space}".format(i))
The question I have now is how do I change and switch around this format??

```.py
# Task One
word = "bear"
for i in range (101):
    print ("bear {0}".format(i))
#how do I do the special case and turn the other way around?

# Task Two
for i in range (1900, 2001, 1):
    print ("The year is {0}". format(i))

# Task Three
for a in range (101):
    for b in range (32.0, 212, 1.8):
        print (format(a), "{0} C are {0}", format (b), "{0} F")
#What does a "float" mean?

```
