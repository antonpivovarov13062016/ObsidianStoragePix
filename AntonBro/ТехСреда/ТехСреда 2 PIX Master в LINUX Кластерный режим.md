

Обеспечивает:
**Отказоустойчивость и производительность.


![[Pasted image 20240713223214.png]]

Мастер хранит в папке keys, если isCluster = true, то в Базе Данных.



![[Pasted image 20240713223531.png]]


![[Pasted image 20240713223547.png]]






![[Pasted image 20240713223617.png]]




Данные Всех Master'ов хранятся в Redis
![[Pasted image 20240713223701.png]]





![[Pasted image 20240713223712.png]]




![[Pasted image 20240713223819.png]]



Могут быть доп сервисы Message Broker и т.д.



![[Pasted image 20240713224134.png]]


![[Pasted image 20240713224142.png]]


Если что-то ломается, **Balancer** переводит запросы на другой Master/

![[Pasted image 20240713224212.png]]

