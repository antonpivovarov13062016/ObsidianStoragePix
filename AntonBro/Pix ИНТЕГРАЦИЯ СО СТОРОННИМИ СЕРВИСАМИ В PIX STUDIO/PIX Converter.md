


## PIX Converter с UiPath на PIX RPA[](https://docs.pixrobotics.com/articles/rpa/converter_uipath/a/h2__289765546 "Link to this heading")

PIX Переходник и PIX Converter с UiPath на PIX RPA  
  
PIX Переходник - программно-методологический комплекс,  
который значительно упрощает перевод проектов RPA с программ зарубежных вендоров на PIX.  
  
PIX Переходник включает в себя:  

- методологию по переходу
- ПО для автоматической конвертации проекта - PIX Converter

PIX Converter - программа, входящая в состав платформы PIX RPA.  
Её можно установить вместе с поставкой релиза PIX Studio 2.8 .

### Возможности PIX Converter (PIX Конвертер):  
[](https://docs.pixrobotics.com/articles/rpa/converter_uipath/a/h3_685564309 "Link to this heading")

- Анализ проекта UiPath с точки зрения конвертируемости - показывает статистику по проекту, анализирует используемые активности и оценивает процент автоматизированного перевода
- Конвертация структуры проекта - все файлы и структура папок будут перенесены в PIX один в один
- Конвертация языка выражений с Visual Basic на C#. Требует дополнительной проверки и редакции после конвертации, но снимает большую часть работы по переводу LINQ-выражений и прочих обработок данных
- Конвертация активностей - 100+ конвертируемых активностей (Базовые, Excel, Email, Web, Desktop, CSV и т.д.)
- Конвертация различных структур проекта - Sequence, Flowchart, StateMachine
- Те шаги, которые пока не конвертируются переносятся в проект PIX в виде комментария с определенной пометкой и всеми известными параметрами, которые были в исходном UiPath-проекте.

![](https://docs.pixrobotics.com/resources/Storage/rpa/converter_uipath/converter_uipath-2023-10-24.png)

### Новые функции PIX Converter (в релизе Studio v.2.9, Converter v.0.9.14):[](https://docs.pixrobotics.com/articles/rpa/converter_uipath/a/h3__1598785544 "Link to this heading")

  
1. Обработка нераспознанных типов данных. Теперь на этапе анализа появилась новая панель "Нераспознанные типы" - для просмотра списка типов данных, которые используются в исходном проекте, но не распознаются при переносе. Кроме анализа этих типов, теперь можно указать замену. И когда произойдет конвертация новый тип подставится взамен старого (+ добавится соответствующий комментарий в теле скрипта). Таким образом, можно сохранить до 80% работ по доработке типов после переноса.

![](https://docs.pixrobotics.com/resources/Storage/rpa/converter_uipath/converter_uipath-2023-10-24-1.png)

2. Статистика по нераспознанным шагам. Добавлена вкладка "Нераспознанные шаги", по которым можно посмотреть активности, не перенесенные Converter. Это позволит на этапе анализа более точно оценить масштаб работ по 3-му этапу конвертации. Также, можно отправлять данную статистику нам, чтобы мы точнее определяли приоритет по новым доработкам.  
  
3. Добавлено логирование действий.  
Теперь информацию по парсингу и переводу проекта можно посмотреть в логах конвертера.  
  
4. Добавлена возможность переводить отдельные скрипты, вместо проекта целиком.  
  
(5) Более 130 активностей распознаёт и конвертирует PIX Converter.  
Добавлены новые разделы для перевода: Images, Secure strings, Hotkeys и пр.  
  
(6) Доработана и улучшена конвертация для следующих блоков: Default-значения переменных, Try/Catch, ElementExist, GetText, TypeText, TypeInto, ExcelInterop, SMTP, DoWhile, InnerStateMachine, FlowChart.