def cat_bmi(bmi):

    if bmi < 19.5: r= "You're underweight"

    elif bmi <= 24.9: r= "You're within the healthy weight range"

    elif bmi <= 29.9: r= "You're overweight"

    elif bmi <= 34.9: r= "You have type 1 obesity"

    elif bmi <= 39.9: r= "You have type 2 obesity"

    else: r= "You have type 3 obesity"

    return r

def imprimir(a):

    print (a["Name"].upper()+" "+a["Surname"].upper()+" "+a["Age"]+" "+a["Weight"]+" "+a["Height"]+" "+a["Direction"].upper()+" "+a["Phone"]+" " + result.upper() + " " + str(a["BMI"]))

print("welcome to the program . .")

person={"Name":"",

        "Surname":"",

        "Age":0,

        "Weight":0,

        "Height":0,

        "Direction":"",

        "Phone":""}

for x in person:

     person[x]=input(f"type your {x} : ")

bmi=round(float(person['Weight'])/((float(person['Height']))**2),2)

person["BMI"]=bmi

result = "bummer"

result=cat_bmi(bmi)

imprimir(person)


