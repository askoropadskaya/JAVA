# JAVA

Необходимо вывести все числа кратные 4 между числами 40 и 60.
Дополнительная сложность: НЕ использовать конструкцию if.
```
    public static void dz1() {
        for (int i = 40; i < 60; i+=4){
             System.out.print(i + " ");
        }
        System.out.println();
    }
```
Дана строка: 
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
Дана строка:
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
    
