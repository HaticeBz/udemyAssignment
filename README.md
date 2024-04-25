age = int(input("Enter your age, please! :"))

if age < 18 :
    print("You can't' enter the nightclub.")
else :
    print("Welcome to the nightclub!")





number = int(input("Enter a number :"))

if number < 0 :
    print("Negative number.")
elif number == 0 :
    print("0")
else :
    print("Positive number.")

    # or

number = int(input("Enter a number :"))
if number >= 0 :
    if number == 0 :
        print("0")
    else :
        print("Positive number.")
else:
    print("Negative number.")




#User Login
systemUsername = "Elena"
systemPassword = 12345

username = input("Enter your username :")
password = int(input("Enter your password :"))

if (username == systemUsername and password != systemPassword) :
    print("Wrong password")
elif (username != systemUsername and password == systemPassword) :
    print("Wrong username")
elif (username != systemUsername and password != systemPassword) :
    print("Wrong username and password")
else :
    print("Welcome to the system!")




#Body Mass Index
weight = int(input("Enter your weight :"))
height = float(input("Enter your height :"))

bodyMassIndex = weight / (height ** 2)

if bodyMassIndex < 18.5 :
    print("You are underweight")
elif (18.5 <= bodyMassIndex < 25) :
    print("You are normal") 
elif (25 <= bodyMassIndex < 30) :
    print("You are overweight")
else :
    print("You are obese")




#Number Comparison
firstNumber = int(input("Enter a number :"))
secondNumber = int(input("Enter the other number :"))
thirdNumber = int(input("Enter the last number :"))

if (firstNumber > secondNumber and firstNumber > thirdNumber) :
    print("The largest number : ",firstNumber)
elif (secondNumber > firstNumber and secondNumber > thirdNumber) :
    print("The largest number : ",secondNumber)
else :
    print("The largest number : ",thirdNumber)




#Exam Score 
firstMidtermScore = float(input("Enter first midterm score :"))
secondMidtermScore = float(input("Enter second midterm score :"))
finalScore = float(input("Enter final score :"))

averageScore = (firstMidtermScore * 30/100 + secondMidtermScore * 30/100 + finalScore * 40/100)

if averageScore >= 90 :
    print("Grade : AA")
elif averageScore >= 85 :
    print("Grade : BA")
elif averageScore >= 80 :
    print("Grade : BB")
elif averageScore >= 75 :
    print("Grade : CB")
elif averageScore >= 70 :
    print("Grade : CC")
elif averageScore >= 65 :
    print("Grade : DC")
elif averageScore >= 60 :
    print("Grade : DD")
elif averageScore >= 55 :
    print("Grade : FD")
else :
    print("Grade : FF")




#Triangle or quadrilateral
shape = input("Is the shape you want to find a triangle or a quadrilateral? :")
triangle = "triangle"
quadrilateral = "quadrilateral"

if shape == triangle:
    firstSide = int(input("Enter the first side :"))
    secondSide = int(input("Enter the second side :"))
    thirdSide = int(input("Enter the third side :"))
    if (firstSide == secondSide == thirdSide) :
        print("The shape is equilateral")
    elif (firstSide == secondSide or firstSide == thirdSide or secondSide == thirdSide) :
        print("The shape is isosceles")
    elif (firstSide != secondSide != thirdSide) :
        print("The shape is scalene")
    else :
        print("The shape is not a triangle")

else :
    firstSide = int(input("Enter the first side :"))
    secondSide = int(input("Enter the second side :"))
    thirdSide = int(input("Enter the third side :"))
    fourthSide = int(input("Enter the fourth side :"))
    if (firstSide == secondSide == thirdSide == fourthSide) :
        print("The shape is square")
    elif (firstSide == secondSide and thirdSide == fourthSide or firstSide == thirdSide and secondSide == fourthSide or firstSide == fourthSide and secondSide == thirdSide) :
        print("The shape is rectangle")
    else :
        print("The shape is any quadrilateral")
