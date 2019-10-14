# Modu-I
#Losujemy liczbe od 1 do 100

from random import randint

los = randint(1,100)

print("Wylosowana liczba to:", los)

twójaPróba = 2

print("Twója liczba to : ", twójaPróba)

if twójaPróba > los:
    print("Niestety liczba za duża :(")
    print("Spróbuj ponownie")
elif twójaPróba < los:
    print("Niestety liczba za mała :(")
    print("Spróbuj ponownie")
else:
    print("GRATULACJE UDAŁO CI SIĘ (づ◔ ͜ʖ◔)づ")
