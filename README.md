# lecture_35_JS_Browser_Document


Говоря о стандартах, у нас есть:  

**Спецификация DOM**  
описывает структуру документа, манипуляции с контентом и события, подробнее на   [Спецификация DOM ](https://dom.spec.whatwg.org.)    
**Спецификация CSSOM**  
Описывает файлы стилей, правила написания стилей и манипуляций с ними, а также то, как это всё связано со страницей,  [подробнее ](https://dom.spec.whatwg.org.)     
**Спецификация HTML**  
Описывает язык HTML (например, теги) и BOM (объектную модель браузера) – разные функции браузера: setTimeout, alert, location и так далее,  [подробнее ](https://html.spec.whatwg.org). Тут берётся за основу спецификация DOM и расширяется дополнительными свойствами и методами.  
Кроме того, некоторые классы описаны отдельно на https://spec.whatwg.org/.  

Пожалуйста, заметьте для себя эти ссылки, так как по ним содержится очень много информации, которую невозможно изучить полностью и держать в уме.  

Когда вам нужно будет прочитать о каком-то свойстве или методе, справочник на сайте Mozilla https://developer.mozilla.org/ru/search тоже очень хороший ресурс, хотя ничто не сравнится с чтением спецификации: она сложная и объёмная, но сделает ваши знания максимально полными.  

Для поиска чего-либо обычно удобно использовать интернет-поиск со словами «WHATWG [термин]» или «MDN [термин]», например https://google.com?q=whatwg+localstorage, https://google.com?q=mdn+localstorage.  

# lecture_36_JS_Document_DOM-дерево

#  [Задачи ](https://github.com/schoolteacherMP/lecture_36_JS_Document_DOM-tree/blob/main/tasks.md)  

Есть 6 основных методов поиска элементов в DOM:  
![image](https://user-images.githubusercontent.com/113675674/219056971-63da34b5-98c2-4a01-a274-a04b9de422c2.png)  

Безусловно, наиболее часто используемыми в настоящее время являются методы querySelector и querySelectorAll, но и методы getElement(s)By* могут быть полезны в отдельных случаях, а также встречаются в старом коде.  

Кроме того:  

-  Есть метод elem.matches(css), который проверяет, удовлетворяет ли элемент CSS-селектору.  
-  Метод elem.closest(css) ищет ближайшего по иерархии предка, соответствующему данному CSS-селектору. Сам элемент также включён в поиск.  

И, напоследок, давайте упомянем ещё один метод, который проверяет наличие отношений между предком и потомком:

-  elemA.contains(elemB) вернёт true, если elemB находится внутри elemA (elemB потомок elemA) или когда elemA==elemB.

