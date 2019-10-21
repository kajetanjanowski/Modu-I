# Modu-I
#Losujemy liczbe od 1 do 100

from random import randint   #biblioteka pozwalająca na generowanie  liczb 
import os                    #biblioteka pozwalająca wyczyścić okno konsoli
import time                  #biblioteka pozwalająca zatrzymac program na okreslony czas


while True:
    try:
        twojaPróba = int(input("\nPodaj swoja liczbe od 1 do 100: ")) #tutaj wpisujemy naszą liczbę , \n przechodzi do następnej lini
        break
    except ValueError: #wyjatek kiedy nie została wprowadzona liczba
        
        print("\nPodaj liczbę smieszku :)")



print("\nTwója liczba to : ", twojaPróba)

los = randint(1,100) #losowana jest liczba całkowita

liczbaPrób = 0 # liczba prób która była potrzebna do odgadnięcia wylosowanej liczby



while twojaPróba != los: #petla z warunkiem że podana liczba jest inna niż wylosowana
    if twojaPróba > los:   
        liczbaPrób += 1 #dodanie do sumy kolejnych prób użytkownika 

        os.system('cls') # czyszczenie konsoli
        print("\nTwója liczba to : ", twojaPróba)
        print("\nNiestety liczba za duża :(")
        print("\nSpróbuj ponownie")
        
        while True:
            try:
                twojaPróba = int(input("\nPodaj swoją liczbę jeszcze raz: "))  # tutaj wpisujemy naszą liczbę
                break
            except ValueError:
                print("\nPodaj liczbę śmieszku :)")

    else :   # w przypadku gdy nasz liczba jest mniejsza niż wylosowana
        liczbaPrób += 1

        os.system('cls')
        print("\nTwója liczba to : ", twojaPróba)
        print("\nNiestety liczba za mała :(")
        print("\nSpróbuj ponownie")
        
        while True:
            try:
                twojaPróba = int(input("\nPodaj swoją liczbę jeszcze raz: "))  # tutaj wpisujemy naszą liczbę
                break
            except ValueError:
                print("\nPodaj liczbę śmieszku :)")

if twojaPróba == los:   # W przypadku gdzy liczby się zgadzają
    os.system('cls')

    liczbaPrób += 1
    print("\n!!! GRATULACJE UDAŁO CI SIĘ (づ◔ ͜ʖ◔)づ !!!")
    print("\nWylosowana liczna było -> " , los)
    print("\nIlość potrzebnych prób to:", liczbaPrób)
    

time.sleep(1) #zatrzymuje program
