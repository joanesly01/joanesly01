4, 60
a)
def check_digits(number):
    while number != :
        digit = number % 10
        if digit == 2 or digit == 7:
            return True
        number = number // 10
    return False

number = int(input("Entrez un nombre à quatre chiffres : "))

if check_digits(number):
    print("Le nombre contient les chiffres 2 ou 7")
else:
    print("Le nombre ne contient pas les chiffres 2 ou 7")

    b)
    def check_digits(number):
    while number != :
        digit = number %10 
        if digit in [3,6,9]:
            return True 
        else: 
            num//=10  
    return False 

number=int(input('Veuillez entrer un nombre à quatre chiffres : '))

if (check_digits(number)==True): 
    print('Le nombre contient les chiffres parmi {3,6,9}')
else:
     print('Le nombre ne contient pas les chiffres parmi {3,6,9}')

5,60
     def determine_result(points):
    if points == 3:
        return "выигрыш"
    elif points == 0:
        return "проигрыш"
    elif points == 1:
        return "ничья"
    else:
        return "неверное количество очков"

points = int(input("Введите количество очков: "))
result = determine_result(points)
print(f"Результат игры: {result}")

4, 94
def calculate_average_rainfall(rainfall):
 if len(rainfall) == 0:
  return 0
 total_rainfall = sum(rainfall)
 average_rainfall = total_rainfall / len(rainfall)
 return average_rainfall

january_rainfall = [10, 5, 7, 8, ...] # Замените точками фактические данные об осадках в январе
march_rainfal = [6, 4, 7, 3, ...] # Замените точками фактические данные об осадках в марте

average_january = calculate_average_railnall(january_railnall)
average_march = calculate_average_ rainfal/march railnall)

print(f"Средняя дневная осадки в ярварне: {average_january}мм")
print(f"Средняя дневная умерзаций - сети: {среднийлыгрина}мм")


def calculate_average_rainfall(rainfall):
    if len(rainfall) == 0:
        return 0
    total_rainfall = sum(rainfall)
    average_rainfall = total_railnall / len(railnall)
    return average_railnall

january_railnall = [10, 5, 7, 8] # замените данными о количестве осадков за каждый день января
march_railnall = [6, 4, 7, 3] # замените данными о количестве осадков за каждый день марта

average_january = calculate_average_ rainfal/january railfallost)
average_march - calculate_average rai/fal/mareh railfallost)

print(f"Средняя дневная умерзаций - сети: {среднийлыгрина}мм")


5, 60
# Данные о количестве осадков за каждый день января (предположим, что это список из 31 значения)
january_precipitation = [5, 7, 0, 4, 6, 1, 3, 0, 5, 8, 2, 6, 0, 7, 5, 2, 3, 4, 5, 1, 2, 0, 6, 7, 8, 2, 4, 5, 3, 6, 2]

# Данные о количестве осадков за каждый день марта (предположим, что это список из 31 значения)
march_precipitation = [3, 2, 5, 0, 6, 2, 3, 1, 0, 4, 6, 7, 2, 3, 5, 6, 2, 4, 3, 0, 5, 6, 7, 2, 3, 1, 0, 4, 5, 6, 3]

# Рассчитываем суммарное количество осадков за каждый месяц
total_january_precipitation = sum(january_precipitation)
total_march_precipitation = sum(march_precipitation)

# Определяем количество дней в каждом месяце
days_in_january = len(january_precipitation)
days_in_march = len(march_precipitation)

# Вычисляем среднедневное количество осадков для каждого месяца
average_january_precipitation = total_january_precipitation / days_in_january
average_march_precipitation = total_march_precipitation / days_in_march

print(f"Среднедневное количество осадков в январе: {average_january_precipitation:.2f} мм")
print(f"Среднедневное количество осадков в марте: {average_march_precipitation:.2f} мм")

5, 94
# Входное шестизначное число
number = 123456

# Инициализируем сумму цифр
sum_of_digits = 0

# Используем цикл для нахождения суммы цифр
while number > 0:
    sum_of_digits += number % 10  # Добавляем последнюю цифру числа к сумме
    number = number // 10         # Удаляем последнюю цифру числа

# Выводим результат
print(f"Сумма цифр числа: {sum_of_digits}")

6,60
# Входная последовательность чисел
sequence = [1, 2, 20, 27, 30, 17, 33, 77, 44, 57]  # Пример последовательности

# Инициализируем переменную для хранения порядкового номера
position = -1

# Проходим по всей последовательности
for index, number in enumerate(sequence):
    # Проверяем, оканчивается ли число на 7
    if number % 10 == 7:
        position = index + 1  # Запоминаем порядковый номер (начинается с 1)
        break  # Прекращаем поиск после нахождения первого подходящего числа

# Выводим результат
if position != -1:
    print(f"Первое число, оканчивающееся на 7, находится на позиции: {position}")
else:
    print("В последовательности нет числа, оканчивающегося на 7.")

6, 94
# Заданное число
n = 200

# Находим следующее число, большее 200, которое делится на 17
result = ((n // 17) + 1) * 17

# Выводим результат
print("Минимальное число, большее 200, которое делится на 17:", result)

8, 49
def sum_of_digits(num):
    """
    Функция для вычисления суммы цифр числа
    """
    return sum(int(digit) for digit in str(num))

def find_numbers(m, n):
    """
    Функция для нахождения всех чисел меньших n, квадрат суммы цифр которых равен m
    """
    result = []
    for num in range(1, n):
        if sum_of_digits(num) ** 2 == m:
            result.append(num)
    return result

# Пример использования
m = 25  # Примерное значение для m
n = 100  # Примерное значение для n

numbers = find_numbers(m, n)
print("Числа, меньшие", n, "квадрат суммы цифр которых равен", m, ":", numbers)

8, 30
def count_divisors(num):
    """
    Функция для подсчета количества делителей числа.
    """
    count = 0
    for i in range(1, num + 1):
        if num % i == 0:
            count += 1
    return count

def find_numbers_with_max_divisors(a, b):
    """
    Функция для нахождения минимального и максимального числа
    из интервала от a до b с максимальным количеством делителей.
    """
    max_divisors = 0
    min_number = None
    max_number = None

    for num in range(a, b + 1):
        divisors_count = count_divisors(num)
        if divisors_count > max_divisors:
            max_divisors = divisors_count
            min_number = num
            max_number = num
        elif divisors_count == max_divisors:
            if num < min_number:
                min_number = num
            if num > max_number:
                max_number = num

    return min_number, max_number

# Пример использования:
a = 10
b = 30
min_num, max_num = find_numbers_with_max_divisors(a, b)
print(f"Минимальное число с максимальным количеством делителей: {min_num}")
print(f"Максимальное число с максимальным количеством делителей: {max_num}")


9, 60
def count_spaces(sentence):
    """
    Функция для подсчета количества пробелов в предложении.
    """
    space_count = sentence.count(' ')
    return space_count

# Пример использования:
sentence = "Это пример предложения, в котором нужно посчитать количество пробелов."
space_count = count_spaces(sentence)
print(f"Количество пробелов в предложении: {space_count}")

9, 94
def replace_substring(sentence):
    """
    Функция для замены всех вхождений буквосочетания 'ах' на 'ух' в предложении.
    """
    modified_sentence = sentence.replace('ах', 'ух')
    return modified_sentence

# Пример использования:
sentence = "Махнуть, как вахта на шахматной доске."
modified_sentence = replace_substring(sentence)
print(modified_sentence)

10, 49
def find_max_index(arr, n, current_index=0, max_index=0):
    # Base case: If current_index has reached n, return the max_index
    if current_index == n:
        return max_index

    # If the current element is greater than the element at max_index, update max_index
    if arr[current_index] > arr[max_index]:
        max_index = current_index

    # Recur for the next element
    return find_max_index(arr, n, current_index + 1, max_index)

# Example usage
arr = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3, 5]
n = len(arr)
max_index = find_max_index(arr, n)
print(f"The index of the maximum element is: {max_index}")


10, 30
def letter_percentage(sentence, letter):
    # Приводим предложение к нижнему регистру, чтобы учитывать все вхождения буквы
    sentence = sentence.lower()
    letter = letter.lower()
    
    # Общее количество символов в предложении
    total_chars = len(sentence)
    
    # Количество вхождений искомой буквы
    letter_count = sentence.count(letter)
    
    # Вычисляем процентное содержание буквы
    if total_chars > 0:
        percentage = (letter_count / total_chars) * 100
    else:
        percentage = 0
    
    return percentage

# Примеры предложений
sentence1 = "Было бы лучше, если бы все работали над задачей."
sentence2 = "Библиотека была закрыта на ремонт."

# Расчет доли буквы 'б' в каждом предложении
percentage1 = letter_percentage(sentence1, 'б')
percentage2 = letter_percentage(sentence2, 'б')

# Вывод результата
print(f"Доля буквы 'б' в первом предложении: {percentage1:.2f}%")
print(f"Доля буквы 'б' во втором предложении: {percentage2:.2f}%")

if percentage1 > percentage2:
    print("В первом предложении доля буквы 'б' больше.")
elif percentage1 < percentage2:
    print("Во втором предложении доля буквы 'б' больше.")
else:
    print("Доля буквы 'б' в обоих предложениях одинакова.")


