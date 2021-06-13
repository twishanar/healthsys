# healthsys
# Healthcare management system
# I have used my friend's names but you can make changes to suit your convinence
import datetime
def getdate():
    return datetime.datetime.now()
def take(k):
    if k==1:
        c = int(input(print("1 for exercise \n 2 for diet plan")))
        if c==1:
         value = input("enter your data")
         with open("sarayu_ex.txt","a") as op:
            op.write(str([str(getdate())])+":"+value+"\n")
            print("successfully entered")
        elif c==2:
         value = input("enter your data")
         with open("sarayu_diet.txt", "a") as op:
            op.write(str([str(getdate())]) + ":" + value + "\n")
            print("successfully entered")
    elif k==2:
        if k == 1:
            c = int(input(print("1 for exercise \n 2 for diet plan")))
            if c == 1:
                value = input("enter your data")
                with open("saketh_ex.txt", "a") as op:
                  op.write(str([str(getdate())]) + ":" + value + "\n")
                  print("successfully entered")
            elif c == 2:
             value = input("enter your data")
             with open("saketh_diet.txt", "a") as op:
                op.write(str([str(getdate())]) + ":" + value + "\n")
                print("successfully entered")
    elif k==3:

            c = int(input(print("1 for exercise \n 2 for diet plan")))
            if c == 1:
                value = input("enter your data")
                with open("nurail_ex.txt", "a") as op:
                  op.write(str([str(getdate())]) + ":" + value + "\n")
                  print("successfully entered")
            elif c == 2:
               value = input("enter your data")
               with open("nurail_diet.txt", "a") as op:
                op.write(str([str(getdate())]) + ":" + value + "\n")
                print("successfully entered")
    elif k==4:
        if k == 1:
            c = int(input(print("1 for exercise \n 2 for diet plan")))
            if c == 1:
                value = input("enter your data")
                with open("pratheek_ex.txt", "a") as op:
                 op.write(str([str(getdate())]) + ":" + value + "\n")
                 print("successfully entered")
            elif c == 2:
               value = input("enter your data")
               with open("pratheek_diet.txt", "a") as op:
                op.write(str([str(getdate())]) + ":" + value + "\n")
                print("successfully entered")
    else:
        print("invalid input")
def retrive(k):
    if k==1:
        c= int(input(print("enter 1 for exercise \n 2 for diet plan")))
        if c == 1:
                        with open("sarayu_ex.txt") as op:
                         for i in op:
                             print(i, end=" ")
        if c==2:
                        with open("sarayu_diet.txt") as op:
                          for i in op:
                              print(i, end=" ")
    elif k==2:
        c = int(input(print("enter 1 for exercise \n 2 for diet plan")))
        if c == 1:
            with open("saketh_ex.txt") as op:
              for i in op:
                print(i, end=" ")
        elif c == 2:
            with open("saketh_diet.txt") as op:
              for i in op:
                print(i, end=" ")
    elif k==3:
        c = int(input(print("enter 1 for exercise \n 2 for diet plan")))
        if c == 1:
            with open("nurail_ex.txt") as op:
              for i in op:
                print(i, end=" ")
        if c == 2:
            with open("nurail_diet.txt") as op:
              for i in op:
                print(i, end=" ")
    elif k==4:
        c = int(input(print("enter 1 for exercise \n 2 for diet plan")))
        if c == 1:
            with open("pratheek_ex.txt") as op:
              for i in op:
               print(i, end=" ")
        if c == 2:
            with open("pratheek_diet.txt") as op:
               for i in op:
                 print(i, end=" ")

    else:
        print("invalid input")








print("welcome to healthcare management system")
a= int(input(print("enter 1 for logging data and enter 2 for retriving data")))
if a==1:
    b= int(input(print("enter: 1 for sarayu \n 2 for saketh \n 3 for nurail \n 4 for pratheek")))
    take(b)
else:
    b = int(input(print("enter: 1 for sarayu \n 2 for saketh \n 3 for nurail \n 4 for pratheek")))
    retrive(b)


