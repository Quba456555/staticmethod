# staticmethod
class Narzedzia:
    @staticmethod
    def suma(a, b):
        return a + b

    @staticmethod
    def roznica(a, b):
        return a - b

    @staticmethod
    def iloczyn(a, b):
        return a * b

    @staticmethod
    def iloraz(a, b):
        if b != 0:
            return a / b
        else:
            return "Nie można dzielić przez zero."

    @staticmethod
    def potega(a, b):
        return a ** b

    @staticmethod
    def silnia(n):
        if n == 0:
            return 1
        else:
            return n * Narzedzia.silnia(n - 1)

    @staticmethod
    def odwrotnosc(a):
        if a != 0:
            return 1 / a
        else:
            return "brak odwrotności zera"

    @staticmethod
    def kwadrat(a):
        return a ** 2

    @staticmethod
    def pierwiastek_kwadratowy(a):
        if a >= 0:
            return a ** 0.5
        else:
            return "Nie można policzyć pierwiastka z liczby ujemnej"

    @staticmethod
    def pole_prostokata(a, b):
        return a * b

# Przykłady użycia metod statycznych
print(Narzedzia.suma(5, 3))  
print(Narzedzia.roznica(5, 3))  
print(Narzedzia.iloczyn(5, 3)) 
print(Narzedzia.iloraz(5, 3))  
print(Narzedzia.potega(5, 3))  
print(Narzedzia.silnia(5))  
print(Narzedzia.odwrotnosc(5))  
print(Narzedzia.kwadrat(3))  
print(Narzedzia.pierwiastek_kwadratowy(5))  
print(Narzedzia.pole_prostokata(5, 3))  
