Bouncing Balls
def bouncingBall(h, bounce, window):
    mom = 1 
    current_height = h
    bounce_height = h * bounce
    while True:
        if bounce_height < window:
            return mom
        bounce_height = bounce_height * bounce
        mom += 2
        
        
