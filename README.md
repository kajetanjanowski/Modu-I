# Modu-I
#Losujemy liczbe od 1 do 100

from random import randint

twojaPróba = int(input("Podaj swoja liczbe od 1 do 100: ")) #tutaj wpisujemy naszą liczbę

print("Twója liczba to : {twojaPróba} ".format(twojaPróba=twojaPróba))

los = randint(1,100) #losowana jest liczba

print("Wylosowana liczba to:", los) # wypisujemy wylosowaną liczbę

if twojaPróba > los:   # w przypadku gdy nasz liczba jest większa niż wylosowana
    print("Niestety liczba za duża :(")
    print("Spróbuj ponownie")

elif twojaPróba < los:   # w przypadku gdy nasz liczba jest mniejsza niż wylosowana
    print("Niestety liczba za mała :(")
    print("Spróbuj ponownie")

else:   # W przypadku gdzy liczby się zgadzaja
    print("GRATULACJE UDAŁO CI SIĘ (づ◔ ͜ʖ◔)づ")
