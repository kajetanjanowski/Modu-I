# Modu-I
#Losujemy liczbe od 1 do 100

from random import randint

los = randint(1,100) #losowana jest liczba

print("Wylosowana liczba to:", los) # wypisujemy wylosowaną liczbę

twójaPróba = 2  #tutaj wpisujemy naszą liczbę

print("Twója liczba to : ", twójaPróba)

if twójaPróba > los:   # w przypadku gdy nasz liczba jest większa niż wylosowana
    print("Niestety liczba za duża :(")
    print("Spróbuj ponownie")

elif twójaPróba < los:   # w przypadku gdy nasz liczba jest mniejsza niż wylosowana
    print("Niestety liczba za mała :(")
    print("Spróbuj ponownie")

else:   # W przypadku gdzy liczby się zgadzaja
    print("GRATULACJE UDAŁO CI SIĘ (づ◔ ͜ʖ◔)づ")
