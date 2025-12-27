print("Привет! Это самы простейший калькулятро на пайтон!")
print("Введи числа в порядке: ЧИСЛО -> ОПЕРАТОР -> ЧИСЛО")
print("Буквы не вбиваем! А то будут проблемы!")
def plus(a, b):
    return a + b
def minus(a, b):
    return a - b
def prov(a, b):
    return a * b
def dele(a, b):
    return a / b
def square(a):
    return a * a
c = input()
p = []
for i in c:
    if i.isalpha():
        raise TypeError("Я же предупреждал!\n"
                        "ТРЕВОГА!!!\n"
                        "5...\n"
                        "4...\n"
                        "3...\n"
                        "2...\n"
                        "1...\n"
                        "БУМ!!!!")
for i in c:
    if i.isdigit():
        p.append(int(i))
if '+' in c:
    print(plus(*p))
elif '-' in c:
    print(minus(*p))
elif '*' in c:
    print(prov(*p))
elif '/' in c:
    print(dele(*p))
elif '^' in c:
    p.remove(2)
    print(square(*p))
