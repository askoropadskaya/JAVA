# JAVA

1.1 Необходимо вывести все числа кратные 4 между числами 40 и 60.
Дополнительная сложность: НЕ использовать конструкцию if.
```
    public static void dz1() {
        for (int i = 40; i < 60; i+=4){
             System.out.print(i + " ");
        }
        System.out.println();
    }
```
1.2 Дана строка: 
String s = “Перестановочный алгоритм быстрого действия”;
необходимо вывести все буквы “о” из этой строки.
Для указанной строки ответ будет “ооооо” (или в столбик)
```
    public static void dz2() {
        String s = "Перестановочный алгоритм быстрого действия";
        for (int i = 0; i < s.length(); i++){
            if (s.charAt(i) == 'о') {
                System.out.print('o');
            }
        }
        System.out.println();
    }
```
1.3 Дана строка:
String s = “Перевыборы выбранного президента”;
необходимо подсчитать количество букв “е” в строке.
Для указанной строки ответ будет 4.
```
    public static void dz3() {
        String s = "Перевыборы выбранного президента";
        int count = 0;
        for (int i = 0; i < s.length(); i++){
            if (s.charAt(i) == 'е') {
                count++;
            }
        }
        System.out.println(count);
    }
 ```   
2.1 Дан массив:
int[] array = {1, 2, 3, 4, 5, 6, 7, 8, 9};
необходимо вывести среднее арифметическое всех значений массива.

Решение:
```
    
    public static void dz21() {
        int [] arr = {1, 2, 3, 4, 5, 6, 7, 8, 9};
        int sum = 0;
        int avg;
        for (int i = 0; i < arr.length; i++){
           sum += arr[i];
        }
        avg = sum / arr.length;
        System.out.println(avg);
    }
```
2.2 Дан массив: 
int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
необходимо вывести количество элементов в массиве.
```
    public static void dz22() {
        int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, -6}};
        int count = 0;
        for (int i = 0; i < array.length; i++){
            for (int j = 0; j < array[i].length; j++) {
                count ++;
            }
        }
        System.out.println(count);
    }
``` 
2.3 Дан массив:
String[][] array = {{“Привет”, “всем”, “кто”}, {“изучает”, “язык”, “программирования”}, {“java”}};
необходимо подсчитать количество строк в массиве которые не содержат буквы “е”.
```
    public static void dz23() {
        String[][] array = {{"Привет", "всем", "кто"}, {"изучает", "язык", "программирования"}, {"java"}};
        int count = 0;
        for (int i = 0; i < array.length; i++){
            for (int j = 0; j < array[i].length; j++) {
                if (!array[i][j].contains("е")){
                    count ++;
                }
            }

        }
        System.out.println(count);
    }
```
7 kyu
Lombok Encapsulation 
===https://www.codewars.com/kata/5a03295680171ffd7b0000c7===
Java:
```
public class EncapsulationDemo {
    private int number;
    private String stringValue;
    private Object anObject;

    public int getNumber() {
        return number;
    }

    public void setNumber(int number) {
        this.number = number;
    }

    public String getStringValue() {
        return stringValue;
    }

    public void setStringValue(String stringValue) {
        this.stringValue = stringValue;
    }

    public Object getAnObject() {
        return anObject;
    }

    public void setAnObject(Object anObject) {
        this.anObject = anObject;
    }

    public EncapsulationDemo() {
    }

    public EncapsulationDemo(int number, String stringValue, Object anObject) {
        this.number = number;
        this.stringValue = stringValue;
        this.anObject = anObject;
    }
}
```
