


**Константин**



см [[ТехСреда 9 Продвинутая разработка активностей Мастер создания активностей]]

![[Pasted image 20240719221207.png]]

Библиотека с базовыми классами

**Базовые вещи**



Класс в библиотеке

**Например активность присвоить - Assign наследуется от Activity.**
**Метод Execute переопределяет метод.**

Атрибуты :
To - Исходящие
Value - входящие данные


![[Pasted image 20240719221640.png]]



**Есть параметры отвечающие за отображение подсказки и описания.** 

![[Pasted image 20240720091735.png]]



**Нужен особенный контейнер (активность с другими активностями).** 
**Например: Закрытие Excel Interop в определенный момент.**

CanHasChilds - активность говорящая, что в ней могут быть другие активности.

![[Pasted image 20240720092137.png]]

![[Pasted image 20240720092216.png]]



То как работает базовая активность
![[Pasted image 20240720092325.png]]



**Цикл в PIX Studio, кастомной активности. Базовая логика.**
Происходят переходы в указанные методы.

![[Pasted image 20240720092423.png]]




**Например цикл FOR**



![[Pasted image 20240720104325.png]]

Добавили строки
![[Pasted image 20240720104453.png]]



**Далее компилируем в dll,  далее подключаем к проекту через PIX Studio. 
!!!!!!!!!!!!! В папку PIX лучше не складывать, т.к. при переносе они не скопируются.** 



![[Pasted image 20240720105304.png]]


![[Pasted image 20240720105339.png]]



![[Pasted image 20240720105744.png]]



![[Pasted image 20240720105831.png]]



![[Pasted image 20240720105856.png]]





**NUGET пакет**

**!!! id делаем максимально уникальным.** 

![[Pasted image 20240720110313.png]]



![[Pasted image 20240720110336.png]]



![[Pasted image 20240720110519.png]]


![[Pasted image 20240720110541.png]]



**Через Nuget его можно будет заливать в Master.**



