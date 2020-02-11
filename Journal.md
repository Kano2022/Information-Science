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

2. What did I learn today?

I realized the pattern and the importance of it and although it was difficult, I enjoyed seeing the program work.

3. Any questions?

How do people manage to make apps??
