# Halloween

def setup(): 
    size(640, 480) 
    background(0)

def draw(): 
    noStroke()
    
    #ground
    fill (101, 67, 33)
    rect(0, height - 200, width, 200)
    stroke (0)
    for x in range (50, 641, 50):
        line(x, 480, x, 280)

    #Pumpkin
    fill(0,255,0)
    noStroke ()
    rect( 360, 240 / 2, 25, 50)
    fill(255, 165, 0)
    ellipse(width *2 /3, height / 2, 200, 200)
    ellipse(width /2, height /2, 200, 200)
    
    #Face
    fill(255, 255, 0)
    stroke(0);
    triangle(270, 220, 350, 220, 310, 160)
    triangle(390, 220, 430, 160, 470, 220)
    triangle(270, 260, 300, 310, 330, 260)
    triangle(300, 310, 365, 310, 330, 260)
    triangle(330, 260, 365, 310, 400, 260)
    triangle(365, 310, 400, 260, 435, 310)
    triangle(400, 260, 435, 310, 470, 260)

    
    
