# -Python-1
1

number1 = int(input('Напишите первое число: '))
number2 = int(input('Напишите второе число: '))
string1 = str(input('Назовите свое имя: '))

print('Вы ввели следующие данные: %d %d %s' % (number1,number2,string1))
print(number1/number2)
print('Моё имя: ' + string1)

numberofsecond = int(input('Введите количество секунд: '))
hour = (numberofsecond//3600)
minute = (numberofsecond - hour*3600)//60
second = numberofsecond - (hour*3600 + minute*60)

print(f"Время в формате чч:мм:сс   {hour:02} : {minute:02} : {second:02}")


numbern = int(input('Введите число n: '))
n = int(numbern)
nn = int(str(numbern) + str(numbern))
nnn = int(str(numbern) + str(numbern) + str(numbern))
print('Сумма чисел: %d + %d + %d =' % (n,nn,nnn) + str(int(n + nn + nnn)))


start = int(input("Результат в первый день, километров: "))
finish = int(input("Необходимо достигнуть, километров: "))
day = 1
while True:
    if start > finish:
        break
    start *= 1.1
    day += 1
print(f"на {day}-й день спортсмен достиг результата — не менее {finish} км.")

number = int(input('Введите целое положительное число: '))
maxnumber = number % 10
while number > 0:
    if number % 10 > maxnumber:
        maxnumber = number % 10
    number = number//10
print('Самая большая цифра в числе: ' + str(int(maxnumber)))


income = int(input('Введите значение прибыли: '))
costs = int(input('Введите значение издержек: '))
profit = income-costs
profitability = profit/income

if income >= costs:
   print('Вы работаете с прибылью:' + str(int(profit)))
   print('Рентабельность вашей работы: ' + str(float(profitability)))
   employees = int(input('Введите численность сотрудников: '))
   profitonemloyees = int(profit/employees)
   print('Прибыль фирмы в расчете на одного сотрудника: ' + str(int(profitonemloyees)))
else:
    print('Вы работаете с убытком:' + str(int(profit)))

    start = int(input('Введите результат первого дня (в км): '))
    target = int(input('Введите минимальный общий результат (в км): '))
    day = int(1)

    start = int(input("Результат в первый день, километров: "))
finish = int(input("Необходимо достигнуть, километров: "))
day = 1
while True:
    if start > finish:
        break
    start *= 1.1
    day += 1
print(f"на {day}-й день спортсмен достиг результата — не менее {finish} км.")
