
см [[ТехСреда 3 PIX Open Office Calc]]
**Пример**:

Нужен робот, который открывает документы *.ods и ищет нужную позицию (цифру после итого).
У каждого менеджера свои данные.

![[Pasted image 20240714122649.png]]


![[Pasted image 20240714124424.png]]


![[Pasted image 20240714122728.png]]


![[Pasted image 20240714122739.png]]

**Получили:**
![[Pasted image 20240714122812.png]]


**Только в XDOCUMENT** 
**doc.Document.Descendants()** - получить список всех наших узлов.


![[Pasted image 20240714123030.png]]


Далее ищем нужный узел:
Лямбда выражением **doc.Document.Descendants(x=>x.Value == "Итого:")** 

![[Pasted image 20240714123628.png]]

Получили якорь Итого:

![[Pasted image 20240714123350.png]]

Обращаемся к элементу справа .NextNode

![[Pasted image 20240714123505.png]]
((System.Xml.Linq.XElement)ItogoNode.NextNode).Attributes()

![[Pasted image 20240714123843.png]]


![[Pasted image 20240714124612.png]]


Получили

![[Pasted image 20240714124054.png]]

**То выбираем нужный атрибут**

**((System.Xml.Linq.XElement)ItogoNode.NextNode).Attributes().Where(x => x.ToString().StartsWith("office:value=") )**

Далее **Result.FirstOrDefault().Value**
