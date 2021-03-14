print("\t\t\tSENDER")

k=int(input("Please enter k value to shift transform:-"))
ch=input("Now please type your message:")
lst=list(ch)
lst2=[]
for i in range(0,len(lst)):
    if(lst[i].isalpha()):
        if(lst[i]!="Z" and lst[i]!="z"):
            val=(ord(lst[i])+k)  #Finding ASCII values and adding the value of k
            lst2.append(chr(val))
        elif(lst[i]=='Z'):
            c='A'
            val=ord(c)+(k-1)
            lst2.append(chr(val))
        elif( lst[i]=='z'):
            c='a'
            val =ord(c)+(k-1)
            lst2.append(chr(val))
    elif(lst[i].isnumeric()):
        lst2.append(int(lst[i])+k)
    elif(lst[i]==" "):
        lst2.append("@")
    else:
        lst2.append(lst[i])


lst2 =  ' '.join(map(str, lst2)) #Join function to convert the elements of the list to String
print("Message sent!!!!!!!!!!")

print("\n\t\t\tRECEIVER")
print("Message Recieved=",lst2)
r_key=int(input("Enter the key to read the original message="))
if(r_key==k):
    print("Message=",ch)
else:
    print("Invalid key!!!,You can't read the message")

