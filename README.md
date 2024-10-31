import pygame ,sys
import time


pygame.init()

WIDTH = 600
HEIGHT  = 600

s=pygame.display.set_mode((WIDTH,HEIGHT))
pygame.display.set_caption("Birthday card")

img=pygame.image.load("birthsign.png")
image = pygame.transform.scale(img, (WIDTH,HEIGHT))

while(True):
    font=pygame.font.SysFont("new year card",72)
    text=font.render("Happy",True,(0,0,0))
    text2=font.render("Birtday",True,(0,0,0))
    s.fill((255,255,255))
    s.blit(image,(0,0))
    s.blit(text,(210,180))
    s.blit(text2,(180,264))
    pygame.display.update()
    time.sleep(2)

    img=pygame.image.load("cake.png")
    image = pygame.transform.scale(img, (WIDTH,HEIGHT))


    font=pygame.font.SysFont("new year card",72)
    text3=font.render("Birthday",True,(0,0,0))
    text4=font.render("Cake",True,(0,0,0))
    s.blit(image,(0,0))
    s.blit(text3,(210,180))
    s.blit(text4,(180,264))
    pygame.display.update()
    time.sleep(2)
    

    img=pygame.image.load("card.png")
    image = pygame.transform.scale(img, (WIDTH,HEIGHT))
    font=pygame.font.SysFont("new year card",72)
    text5=font.render("This",True,(0,0,0))
    text6=font.render("is your birthday card",True,(0,0,0))
    s.blit(image,(0,0))
    s.blit(text5,(210,180))
    s.blit(text6,(180,264))
    pygame.display.update()
    time.sleep(2)
    
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    


