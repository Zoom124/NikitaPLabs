[Ссылка на борд](https://repl.it/@NikitaPopov/20-09-18)

Код:

lst = [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, 10946]

# https://repl.it/@zhukov/20-09-18
# Сумму четных элементов (со второго по предпоследний элемент) списка.
s = 0;
for i in lst[1:len(lst)-1]:
  if  i%2==0:s+=i
print(s)
# Сумму нечетных элементов (с пятого по предпредпоследний элемент) списка.
s = 0;
for i in lst[4:len(lst)-1]:
  if  i%2==1:s+=i
print(s)
# Сумму элементов, расположенных на четных позициях, первой половины списка.
print(sum(lst[:len(lst)//2:2]))
# Сумму элементов, расположенных на нечетных позициях, второй половины списка.
print(sum(lst[len(lst)//2::2]))
# Максимальный элемент, стоящий на четной позиции среди элементов второй половины списка.
print(max(lst[len(lst)//2+1::2]))
# Минимальный элемент, стоящий на нечетной позиции среди элементов первой половины списка.
print(min(lst[1:len(lst)//2:2]))
# Список элементов, стоящих на четных позициях во второй половине списка в обратном порядке.
print(lst[:len(lst)//2-1:-1][1::2])