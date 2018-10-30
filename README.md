colour1 = 255
colour2 = 165
center = 374 
centery = 243
clicked = False
def setup():
    size(640, 480)
    
def draw():
    global colour1
    global colour2
    background(0)
    noStroke()
   #Pumpkin
    fill(0,colour1,0)
    rect( 360, 240 / 2, 25, 50)
    fill(colour1, colour2, 0)
    ellipse(width *2 /3, height / 2, 200, 200)
    ellipse(width /2, height /2, 200, 200)

    #Face
    fill(colour1, colour1, 0)
    stroke(0);
    triangle(270, 220, 350, 220, 310, 160)
    triangle(390, 220, 430, 160, 470, 220)
    triangle(270, 260, 300, 310, 330, 260)
    triangle(300, 310, 365, 310, 330, 260)
    triangle(330, 260, 365, 310, 400, 260)
    triangle(365, 310, 400, 260, 435, 310)
    triangle(400, 260, 435, 310, 470, 260)
    
    #fading
    if clicked == True:
        colour1 -= 2
        colour2 -= 2

def mouseClicked():
    global clicked
    clicked = True
