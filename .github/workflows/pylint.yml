

def fitnessTracker():
    login = True
    username = ''
    while (login == True):
        username = input("Please enter your username: ")
        if (username == 'Shreya'):
            username = 'Shreya'
            password = input("Please enter your password: ")
            if (password == '123456'):
                login = False
            else:
                print("Password incorrect!")
        else:
            print("Username incorrect!")

    if (login == False):
        flag = 1;
        while (flag == 1):
            print('Welcome to Fitness Tracker')
            print('Track yourself on the basis of:')
            print('1.Workout')
            print('2.BMI')
            print('3.WaterIntake')
            print('4.BMR')
            print('5.CalorieBurnedApprox')
            print('Please select the option by entering serial number')
            int
            serialNumber = int(input())
            if (serialNumber == 1):
                main()
            if (serialNumber == 2):
                BMI()
            if (serialNumber == 3):
                waterIntake()
            if (serialNumber == 4):
                BMR()
            if (serialNumber == 5):
                approxCalorieBurned()
            flag = int(input('Want to continue , enter 1 for yes and 0 for No'))
        print('Thanks for using fitness tracker')


def getTime(type):
    did_ = input('Did you do ' + type + '? (yes/no): ')
    if did_.lower() == 'no':
        return 0
    else:
        time = float(input('Enter how long you did ' + type + '? (mins): '))
        return time


def main():
    totalTime = [0, 0, 0]
    types = ['yoga', 'cardio', 'meditation']
    days = input("enter your day :")

    for type in types:
        time = getTime(type)
        if type == 'yoga':
            totalTime[0] += time
        elif type == 'cardio':
            totalTime[1] += time
        else:
            totalTime[2] += time




    if sum(totalTime) >= 3 * 20 * 1:
        print('Your fitness score is 5 on scale of 5.0')
    elif sum(totalTime) >= 3 * 20 * 1 * 0.8:
        print('Your fitness score is 4 on scale of 5.0')
    elif sum(totalTime) >= 3 * 20 * 1 * 0.6:
        print('Your fitness score is 3 on scale of 5.0')
    elif sum(totalTime) >= 3 * 20 * 1 * 0.4:
        print('Your fitness score is 2 on scale of 5.0')
    else:
        print('Your fitness score is 1 on scale of 5.0')


def BMI():
    the_height = float(input("Enter the height in cm: "))
    the_weight = float(input("Enter the weight in kg: "))
    the_BMI = the_weight / (the_height / 100) ** 2
    if the_BMI < 18.5:
        print("Your Body Mass Index is", the_BMI)
        print('Underweight')
    if the_BMI >= 18.5 and the_BMI < 25:
        print("Your Body Mass Index is", the_BMI)
        print("Normal")
    if the_BMI >= 25 and the_BMI < 30:
        print("Your Body Mass Index is", the_BMI)
        print('Overweight')
    if the_BMI >= 30:
        print("Your Body Mass Index is", the_BMI)
        print('Obesity')


def waterIntake():
    the_weight = float(input("Enter the weight in kg: "))
    age = int(input("Enter the age: "))
    the_weight = the_weight * 2.20462
    if (age < 30):
        water_intake = the_weight * 40
    elif (age >= 30 and age < 55):
        water_intake = the_weight * 35
    elif (age >= 55):
        water_intake = the_weight * 30

    water_intake = water_intake / 28.3
    water_intake = water_intake * 0.0295735
    print('The water required for you will be : ', water_intake)


def BMR():
    the_height = float(input("Enter the height in cm: "))
    the_weight = float(input("Enter the weight in kg: "))
    age = int(input("Enter the age: "))
    gender = input('Enter gender (M/F)')
    if (gender == 'M'):
        bMR = 66 + (6.2 * the_weight) + (12.7 * the_height) - (6.76 * age)
    else:
        bMR = 655.1 + (4.35 * the_weight) + (4.7 * the_height) - (4.7 * age)
    print('BMR calculated is: ', bMR)
    return bMR


def approxCalorieBurned():
    value = BMR()
    print('1.little to no exercise')
    print('2.light exercise 1–3 days a week')
    print('3.moderate exercise 3–5 days a week')
    print('4.exercises hard 6–7 days a week')
    print('5.extra active person ')
    exercise = int(input('Select your activity level:'))
    if (exercise == 1):
        print('Calorie need to burn for maintaining weight :', value * 1.2)
    if (exercise == 2):
        print('Calorie need to burn for maintaining weight :', value * 1.37)
    if (exercise == 3):
        print('Calorie need to burn for maintaining weight :', value * 1.55)
    if (exercise == 4):
        print('Calorie need to burn for maintaining weight :', value * 1.725)
    if (exercise == 5):
        print('Calorie need to burn for maintaining weight :', value * 1.9)
    
    approxCalorieBurned()

fitnessTracker()
