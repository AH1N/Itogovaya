# Описание решения задачи из итоговой контрольной работы


**Описание задачи :**
```
Написсать программу, которая из имеющегося массива строк, формирует массив мз строк, длина которых не привышает заданного значения(тут 3). Первоначальный массив можно задать на старте, либо ввести с клавиатуры. При решении не рекомендектся пользоваться коллекциями, лучше обойтисьб только массивами
```
**Решение**
1) задать массив на старте *String[] textArray*;
2) создать методы помогающие решать поставленную задачу
    - метод проверяющий/сортирующий элементы исходного массива ***string SortElementsInCurrentArray(
	string[] array, 
	int placeOfelement, 
	int numOfSymbolsInElement)***


    - метод создающий новый массив из подходящих элементов изходного ***CreateNewArrayFromCurrentArray(
    string[] array, 
    int numOfSymbolsInElement)***;

    - метод распечатывающий массив ***Void PrintArr()***;

Метод ***string SortElementsInCurrentArray()*** 
используем внутри метода ***CreateNewArrayFromCurrentArray()***;

**Примечание - 1:**  
``` Метод string SortElementsInCurrentArray() может вернуть элементы со значением <string.Empty>. Необходимо сделать проверку при заполнении результирующего массива. ```

**Примечание - 2:**  
``` Метод PrintArr(), на вход может получить пустой массив, результатом будет ошибка. Неободимо в нутри метода сделать проверку длинны массива, если длинна < 0, вывести сообщение: "Нечего распечатывать", в противном случае распечатать массив.  ```


**Алгоритм выполнения задачи**

![apple](Algorithm.png)