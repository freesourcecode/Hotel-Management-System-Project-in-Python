# Hotel Management System Project in Python with Source Code

The **Hotel Management System Project in Python** is a general software developed (using Python) to simplify hotel operations by automating them.

The system covers major aspects of hotel management, it could perform the following operations. 

Hotel Booking, provides you with Hotel Rooms Info, Room Service, Billing, and Record-Keeping.

* **Hotel Booking**

Function to book a room in a hotel by entering information about the user or customer.

* **Room Management**

This feature manages all the information about the rooms in the hotel.

* **Room Services**

The function the user has to select and give users and customers information about hotel rooms (i.e. about room amenities).

* **Billing and Record-Keeping**

At check-out, there is a function that lets you pay for your hotel room and calculate your restaurant bill.

Use this function to keep track of who has stayed at the hotel and calculate room rent.

----

You don’t have to worry because I will expect that I will guide you to the step-by-step process especially, in declaring it variables and modules.

To start creating this Simple Hotel Management System Project In Python, make sure you have PyCharm IDE and installed Python in your computer.

## How to create a Hotel Management System Project in Python?

1. **Create a Project Name.**

Open the PyCharm IDE and click “File” and select “New Project” and then create a project name after that click the “create” button.

2. **Create a Python File.**

After creating a project name, “right” click the project name and the click “New” after that choose “Python File“.

3. **Name the Python File.**

Third step after choose Python File name the file “Hotel Management System” and then click “Enter”.

4. **The actual code.**

Now you can start coding, you are free to copy the code that being provided below.

Hotel Management Python Code Explanations

1. Class Declaration, Module and Variables

The code given below, which declaring the class , module and its variable.

You are free to copy and paste this code on your Python File.

```
class hotelmanage:

    def __init__(self,rt='',s=0,p=0,r=0,t=0,a=1000,name='',address='',cindate='',coutdate='',rno=1):

        print ("\n\n*****WELCOME TO HOTEl DE SUAREZ*****\n")

        self.rt=rt

        self.r=r

        self.t=t

        self.p=p

        self.s=s
        self.a=a
        self.name=name
        self.address=address
        self.cindate=cindate
        self.coutdate=coutdate
        self.rno=rno
```
2. **Customer Information**

This module ask the system to the user to enter the data or information of the customer.

```
def inputdata(self):
        self.name=input("\nEnter your Fullname:")
        self.address=input("\nEnter your address:")
        self.cindate=input("\nEnter your check in date:")
        self.coutdate=input("\nEnter your checkout date:")
        print("Your room no.:",self.rno,"\n")
```

3. **Room Rent**

This module displayed the type of rooms that you want to choose and their specific price.


```
def roomrent(self):#sel1353

        print ("We have the following rooms for you:-")

        print ("1.  Class A---->4000")

        print ("2.  Class B---->3000")

        print ("3.  Class C---->2000")

        print ("4.  Class D---->1000")

        x=int(input("Enter the number of your choice Please->"))

        n=int(input("For How Many Nights Did You Stay:"))

        if(x==1):

            print ("you have choose room Class A")

            self.s=4000*n

        elif (x==2):

            print ("you have choose room Class B")

            self.s=3000*n

        elif (x==3):

            print ("you have choose room Class C")

            self.s=2000*n

        elif (x==4):
            print ("you have choose room Class D")

            self.s=1000*n

        else:

            print ("please choose a room")

        print ("your choosen room rent is =",self.s,"\n")
```

4. **Food Module**

In this module displayed the list of foods and thier specific price to be order by the customer.

```
 def foodpurchased(self):

        print("*****RESTAURANT MENU*****")

        print("1.Dessert----->100","2.Drinks----->50","3.Breakfast--->90","4.Lunch---->110","5.Dinner--->150","6.Exit")


        while (1):

            c=int(input("Enter the number of your choice:"))


            if (c==1):
                d=int(input("Enter the quantity:"))
                self.r=self.r+100*d

            elif (c==2):
                 d=int(input("Enter the quantity:"))
                 self.r=self.r+50*d

            elif (c==3):
                 d=int(input("Enter the quantity:"))
                 self.r=self.r+90*d

            elif (c==4):
                 d=int(input("Enter the quantity:"))
                 self.r=self.r+110*d

            elif (c==5):
                 d=int(input("Enter the quantity:"))
                 self.r=self.r+150*d

            elif (c==6):
                break;
            else:
                print("You've Enter an Invalid Key")

        print ("Total food Cost=Rs",self.r,"\n")
```

5. **Billing Module**

In this module displayed the total purchased of the customer.

```
def display(self):
        print ("******HOTEL BILL******")
        print ("Customer details:")
        print ("Customer name:",self.name)
        print ("Customer address:",self.address)
        print ("Check in date:",self.cindate)
        print ("Check out date",self.coutdate)
        print ("Room no.",self.rno)
        print ("Your Room rent is:",self.s)
        print ("Your Food bill is:",self.r)

        self.rt=self.s+self.t+self.p+self.r

        print ("Your sub total Purchased is:",self.rt)
        print ("Additional Service Charges is",self.a)
        print ("Your grandtotal Purchased is:",self.rt+self.a,"\n")
        self.rno+=1
```

### 📌 Here's the full documentation for the [Medical Store Management System Project in Python](https://itsourcecode.com/free-projects/python-projects/hotel-management-system-project-in-python/)
