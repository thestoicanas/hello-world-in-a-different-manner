# hello-world using string and time delays manipulation


# This Programme uses string and time manipulation to print the hello world





import string
import time

text = 'Hello world'  # printable text
temp = ''           # builds the string character by character

for ch in text:     # Loop through each character in the target text
    # random characters until hits the correct one
    for i in string.printable:  # Try every printable character
        if i == ch:             # If we found the correct character
            temp += ch          # Add the correct character to temp
            print(temp, end='\r') #or print(temp)   # Print the current string (overwrite line)
            time.sleep(0.05)    # pauses after correct character
            break               
        else:
            # prints wrong programme
            print(temp + i, end='\r') #or print (temp)
            time.sleep(0.02)    # Fast flicker for wrong attempts

# Final line breaks
print()  # new line
print("Final text:", text)
