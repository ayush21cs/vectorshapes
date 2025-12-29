# VectorShapes
A flexible, easy-to-use python module for pygame for rendering vector-based shapes with dynamic video, textures and random colours as well as smooth color transformations.
## Features
- easy to use, just import module, make object and render
- no calculation needed, just origin, lenght, breadth and height needed for simplest cuboid
- multiple color options, you can set front,top and right side colors manually or use attributes for random color generation or constant transformations
- video(s) can be displayed very easily
- many other features are included
- made from scratch
## Demo
youtube link is yet to be inserted here
## Installation
One must pip install pygame and cv2 modules. otherwise it will not work.
## Basic Example
import pygame; pygame.init()
import vectorshapes as vs  #import module(should be in same file, file name should also be correct)
screen = pygame.display.set_mode((2560,1440))
clock = pygame.time.Clock()
run = True
cube = vs.UltraCuboid((100,100),100,200,300) #make a cuboid
while run:
    screen.fill((0,0,0))
    mx,my = pygame.mouse.get_pos()
    k = pygame.key.get_pressed()
    for e in pygame.event.get():
        if e.type == pygame.QUIT or k[pygame.K_ESCAPE]:
            run = False
    cube.render() #render
    pygame.display.flip()
    clock.tick(100)
pygame.quit()
## Media Disclaimer
This project does not contain anu video files.
User must supply their own video files and ensure they have the rights to use them.
## License
MIT Licence
## Author
Created by ayush21cs
