
[[ТехСреда 2 PIX Master Docker]]



![[Pasted image 20240713221459.png]]


![[Pasted image 20240713221519.png]]

Только чистый трафик HTTP идет на мастер



![[Pasted image 20240713221702.png]]


![[Pasted image 20240713221714.png]]



![[Pasted image 20240713221723.png]]



![[Pasted image 20240713221733.png]]
!!!!!!!!!!!!!!!!!!!!
	**Даем полный доступ 777 к папкам keys и masterlog**





![[Pasted image 20240713222021.png]]


![[Pasted image 20240713222028.png]]

Настраиваем

![[Pasted image 20240713222039.png]]

![[Pasted image 20240713222047.png]]



![[Pasted image 20240713222058.png]]



**Если PIX MASTER не локальный:**
	Указываем ip и port PIX MASTER
	![[Pasted image 20240713222155.png]]
	Нужно получить сертификат подписанный хостинг провайдером



**HTTPD**

![[Pasted image 20240713222456.png]]



**Не запустятся web-soket'ы если не написать websocket маленькими буквами**

![[Pasted image 20240713222747.png]]


![[Pasted image 20240713222802.png]]


![[Pasted image 20240713222514.png]]




![[Pasted image 20240713222529.png]]

**ЕСЛИ**
**На одном сервере нужно запустить несколько master'ов**.
То.
Создаем каждый сервис на своем порту 5000 , 5050 и т.д.

![[Pasted image 20240713222919.png]]


![[Pasted image 20240713222935.png]]



[[ТехСреда 2 PIX Master в LINUX Кластерный режим]]






