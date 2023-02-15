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
