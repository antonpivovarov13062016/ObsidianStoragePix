

Нужна чтобы Master'a могли между собой общаться и понимали какие процессы выполняются
Правильно ставить БД и Redis в кластерном режиме для отказоутойчивости.


![[Pasted image 20240714171019.png]]


![[Pasted image 20240714173525.png]]

![[Pasted image 20240714173519.png]]



![[Pasted image 20240714173245.png]]



![[Pasted image 20240714173753.png]]


1


![[Pasted image 20240714173831.png]]


2

![[Pasted image 20240714173844.png]]


3


![[Pasted image 20240714173856.png]]




![[Pasted image 20240714173954.png]]


![[Pasted image 20240714174013.png]]




![[Pasted image 20240714174050.png]]


4

![[Pasted image 20240714174110.png]]


5


![[Pasted image 20240714174149.png]]

![[Pasted image 20240714174218.png]]

**6**

**Подключаем Мастер к Redis**

Для этого отключаемся
![[Pasted image 20240714174301.png]]


![[Pasted image 20240714174416.png]]



![[Pasted image 20240714174445.png]]



7

![[Pasted image 20240714174510.png]]


8

Правим appettings.json

![[Pasted image 20240714174554.png]]


9
Подключение через dotnet Master.dll к Мастеру дает больше логов


![[Pasted image 20240714174700.png]]


10  **Запуск в нормальном режиме**

![[Pasted image 20240714174833.png]]


11 Проверяем


![[Pasted image 20240714174914.png]]


