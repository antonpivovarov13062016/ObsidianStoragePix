
см [[ТехСреда 3 PIX Open Office Calc]]
**Валентин Дроздов** Менеджер продукта PIX RPA
**Кирилл Пронин** Разработчик PIX RPA



![[Pasted image 20240714110145.png]]




**Работа с таблицами происходит в памяти робота**

![[Pasted image 20240714110520.png]]


За счет паттерна достигается гибкость
![[Pasted image 20240714110618.png]]


**С помощью npoi(открытый код) общаемся напрямую.**
**!! npoi округляет числа в большую сторону, Excel в меньшую**

![[Pasted image 20240714110713.png]]



**Обращаемся к приложению Microsoft Excel (отдельное приложение).**

![[Pasted image 20240714110847.png]]



Считывает так, как это видит пользователь.
Нужно открыть, считать диапазон и **закрыть**
![[Pasted image 20240714111029.png]]




![[Pasted image 20240714111338.png]]

npoi  поддерживает XLS, но не стабильно


**Проблема больших таблиц**




![[Pasted image 20240714111759.png]]


![[Pasted image 20240714111827.png]]




![[Pasted image 20240714111840.png]]








![[Pasted image 20240714112542.png]] 


![[Pasted image 20240714112646.png]]



![[Pasted image 20240714112632.png]]



**Пример:**



Код для Interop

![[Pasted image 20240714114946.png]]




![[Pasted image 20240714112830.png]]


![[Pasted image 20240714112812.png]]



![[Pasted image 20240714112947.png]]



![[Pasted image 20240714113039.png]]


![[Pasted image 20240714113106.png]]



![[Pasted image 20240714113206.png]]

Но 
![[Pasted image 20240714113227.png]]


**Обязательно**

![[Pasted image 20240714113129.png]]



**В NPOI**

Разница в отображении.
![[Pasted image 20240714113243.png]]



1. Запускаем приложение Excel
2. Получаем значения и заносим в cell

![[Pasted image 20240714113857.png]]

**Используем Value2**

Код вносим в активность 

![[Pasted image 20240714114147.png]]


Удобный код для считывания разных типов ячеек. Высокая сложность.

![[Pasted image 20240714115255.png]]



![[Pasted image 20240714115642.png]]

