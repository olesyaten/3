# Пример кода на Python: Калькулятор

def add(a, b):
    """Функция для сложения двух чисел"""
    return a + b

def subtract(a, b):
    """Функция для вычитания второго числа из первого"""
    return a - b

def multiply(a, b):
    """Функция для умножения двух чисел"""
    return a * b

def divide(a, b):
    """Функция для деления первого числа на второе"""
    if b == 0:
        raise ValueError("На ноль делить нельзя!")
    return a / b

if __name__ == "__main__":
    print("Калькулятор")
    num1 = float(input("Введите первое число: "))
    num2 = float(input("Введите второе число: "))

    print(f"{num1} + {num2} = {add(num1, num2)}")
    print(f"{num1} - {num2} = {subtract(num1, num2)}")
    print(f"{num1} * {num2} = {multiply(num1, num2)}")
    try:
        print(f"{num1} / {num2} = {divide(num1, num2)}")
    except ValueError as e:
        print(e)
