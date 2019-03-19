
            yspeed = -yspeed
        if pos[2] >= WIDTH or pos[0] <= 0:
            xspeed = -xspeed
    
        canvas.move(ball2, xspeed2, yspeed2)
        pos = canvas.coords(ball2)
        if pos[3] >= HEIGHT or pos[1] <= 0:
            yspeed2 = -yspeed2
        if pos[2] >= WIDTH or pos[0] <= 0:
            xspeed2 = -xspeed2

        root.update()
        time.sleep(0.01)

b = Button(root, text= "Click", command=buttonfunction)
b.place(x=50, y=150, width=50, height=50)
        
root.mainloop()


