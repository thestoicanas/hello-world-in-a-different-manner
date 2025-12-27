# hello-world-in-a-different-manner
This Programme prints hello world but not as you think...


import string
import time
text = "Hello World" # go touch the grass
temp = ''
for ch in text:
    for i in string.printable:
        if i == ch or ch == "":
            time.sleep(0.01)
            print(temp+i)
            temp +=ch
            print(temp,) # end='\r')
            break
        else:
            time.sleep(0.02)
            print(temp+i,) #end='\r')
