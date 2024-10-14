
# Ответы на вопросы из 2 теста Чабанова

## Вопросы
- Дан фрагмент кода на языке С++. Будет ли код работать?
```cpp
int main(){
    print(1, 2, " ");
}

void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ: <code> Нет. Ошибка на этапе компиляции </code>

- Язык Go. Выберите все верные утверждения касающиеся оператора return в теле функции:<br>

Ответ: <code>Может отсутствовать в некоторых функциях;</code></br>
<code>Может быть указан в теле функции более одного раза;</code></br>
<code>Прерывает исполнение функции и возвращает поток исполнения в точку вызова;</code>

- Код на языке С++. Выберите все позиции (отмеченные комментарием) в которых разрешено объявлять функцию sum.
```cpp
// 1
#include <iostream>
// 2
int main(){
    // 3
    std::cout << "Don't blink" << std::endl;
    // 4
}
// 5

int sum(int a, int b){
    // 6
    return a + b;
    // 7
}
// 8
```
Ответ: <code> 1 2 3 4 5 6 7 8 </code>

- Дана функция на языке С++. Выберите все варианты вызова данной функции, при которых произойдёт обмен значениями переменных x и y. Переменные обвялены следующим образом: int x = 1; и int y = 2;:
```cpp
void swap(int& a, int& b){
    int t = a;
    a = b;
    b = t;
}
```
Ответ: <code> swap(y, x); </code><br>
<code> swap(x, y); </code>

- Дана функция на языке С++. Выберите все варианты вызова данной функции, при которых произойдёт обмен значениями переменных x и y. Переменные объявлены следующим образом: int x = 1; и int y = 2;:
```cpp
void swap(int* a, int* b){
    int t = *a;
    *a = *b;
    *b = t;
}
```
Ответ: <code>swap(&x, &y);</code><br>

- Дан фрагмент код на на языке Go. Что будет на экране в результате его выполнения:
```go
package main
import "fmt"

func print(){
    fmt.Println(a)
}

func main(){
    a := 10
    print()
}
```
Ответ: <code>Ошибка во время компиляции;</code>

- Язык С++. Выберите все верные утверждения касающиеся оператора return в теле функции:<br>

Ответ: <code>Может отсутствовать в некоторых функциях;</code></br>
<code>Прерывает исполнение функции и возвращает поток исполнения в точку вызова;</code></br>
<code>Может быть указан в теле функции более одного раза;</code>

- Дана функция на языке Go. Выберите все верные утверждения:
```go
func min(a, b int) int{
    if a < b {
        return a
    }
    return b
}
```
При условии, что функция вызывается так:
```go
x, y := 10, 0
min(x, y)
```
Ответ: <code>Параметры функции получает локальную копию аргументов;</code><br>
<code>Функция принимает аргументы по значению;</code>

- Дана функция на языке Go. Выберите все варианты вызова данной функции, при которых произойдёт обмен значениями переменных x и y. Переменные объявлены следующим образом: x := 1; и y := 2;:
```go
func swap(a, b int){
    var t int = a
    a = b
    b = t
}
```
Ответ: <code>Эта функция не может выполнить требуемое действие;</code>

- Дана функция на языке С++. Выберите все верные утверждения:
```cpp
int mydiv(int a, int b){
    int result = a % b;
    return result;
}
```
При условии, что функция вызывается так:
```cpp
int x = 9, y = 2;
int z = mydiv(x, y);
```
Ответ: <code> В точке вызова будет создана копия локальной переменной result или произойдёт оптимизация (RVO, NRVO);</code><br>
<code> Функция возвращает результат по значению;</code>

- Дана функция на языке С++. Выберите все верные утверждения:
```cpp
int min(int& a, int& b){
    return a < b ? a : b;
}
```
При условии, что функция вызывается так:
```cpp
int x = 10, y = 0;
min(x, y);
```
Ответ: <code>Функция принимает аргументы по ссылке;</code><br>
<code> Параметры функции становятся вторыми именами для переменных x и y;</code>

- Код на языке С++. Выберите все позиции (отмеченные комментарием) в которых можно объявить функцию sum, чтобы сделать код рабочим.
```cpp
// 1
#include <iostream>
// 2
int main(){
    // 3
    std::cout << sum(2, 2) << std::endl;
    // 4
}
// 5

int sum(int a, int b){
    // 6
    return a + b;
    // 7
}
// 8
```
Ответ: <code>1 2 3</code>

- Дан фрагмент кода на С++. Что будет напечатано в результате его выполнения?
```cpp
int i = 1;

int main() {
    std::cout << i;
    int i = 2;
    {
        std::cout << i;
        int i = 3;
    }
    std::cout << i;
}
```
Ответ: <code>122</code>

- Язык Go. Функция задана сигнатурой:
```go
func maxmin(a, b float64) (max float64, min float64)
```
Каким образом можно выйти из этой функции?<br>

Ответ: <code>return без значений</code><br>
<code>return с двумя значениями</code>

- Дан фрагмент код на на языке С++. Что будет на экране в результате его выполнения:
```cpp
void print(){
    std::cout << a;
}

int main(){
    int a = 10;
    print();
}
```
Ответ: <code>Ошибка во время компиляции;</code>

- Язык Go. Выберите сигнатуры всех функций, для которых обязательно наличие оператора return в теле:<br>

Ответ:
```go
func next() float64
```
```go
func strip(src *string) *string
```
```go
func sum(a, b int) int
```

- Сколько раз, в коде на языке С++, можно писать определение этой функции?
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ: <code>Только один раз в программе;</code>

- Дана функция на языке Go. Выберите все варианты вызова данной функции, при которых произойдёт обмен значениями переменных x и y. Переменные объявлены следующим образом: x := 1; и y := 2;:
```cpp
func swap(a, b *int){
    var t int = *a
    *a = *b
    *b = t
}
```
Ответ: <code>swap(&x, &y);</code>

- Дана функция на языке С++. Выберите всё варианты, которые являются вызовом этой функции:
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ: 
```cpp
print(a, b, sep);
```

- Сколько раз, в коде на языке С++, можно писать объявление этой функции?
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ: <code>Любое количество раз;</code>

- Дана функция на языке Go. Выберите все верные утверждения:
```go
func mydiv(a, b int) int{
    result := a % b
    return result
}
```
При условии, что функция вызывается так:
```go
x, y := 9, 2
z := mydiv(x, y)
```
Ответ: <code>Функция возвращает результат по значению;</code><br>
<code>В точке вызова будет создана копия локальной переменной result;</code>

- Дана функция на языке Go. Выберите все верные утверждения:
```go
func min(a, b *int) int{
    if a < b {
        return a
    }
    return b
}
```
При условии, что функция вызывается так:
```go
x, y := 10, 0
min(&x, &y)
```
Ответ: <code>Функция возвращает результат по значению;</code><br>
<code>Функция принимает аргументы по указателю;</code>

- Код на языке С++. Выберите все позиции (отмеченные комментарием) в которых можно определить функцию sum, чтобы сделать код рабочим.
```cpp
// 1
#include <iostream>
// 2
int main(){
    // 3
    std::cout << sum(2, 2) << std::endl;
    // 4
}
// 5
```
Ответ: <code>1 2</code>

- Код на языке Go. Выберите все позиции (отмеченные комментарием) в которых можно определить функцию sum, чтобы сделать код рабочим.
```go
// 1
package main
// 2
import "fmt"
// 3
func main() {
    // 4
    fmt.Println(sum(2, 2))
    // 5
}
// 6
```
Ответ: <code>3 6</code>

- Код на языке С++. Выберите все позиции (отмеченные комментарием) в которых можно определить функцию sum, чтобы сделать код рабочим.
```cpp
int min(int a, int b){
    return a < b ? a : b;
}
```
При условии, что функция вызывается так:
```cpp
int x = 10, y = 0;
min(x, y);
```
Ответ: <code>Параметры функции получает локальную копию аргументов;</code><br>
<code>Функция принимает аргументы по значению;</code>

- Дан фрагмент кода на Go. Что будет напечатано в результате его выполнения?
```go
package main
import "fmt"

var i int = 1

func main() {
    fmt.Print(i)
    var i int = 2;
    {
        fmt.Print(i)
        var i int = 3;
    }
    fmt.Print(i)
}
```
Ответ: <code>Ошибка</code>

- Дан фрагмент кода на Go. Что будет напечатано в результате его выполнения?
```cpp
void print(short a, short b, std::string sep);

int main(){
    print(1, 2, " ");
}

void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ: <code>Да. Ошибок нет;</code>

- Дана функция на языке Go. Выберите все верные утверждения:
```go
func mydiv(a, b int) *int{
    result := a % b
    return &result
}
```
При условии, что функция вызывается так:
```go
x, y := 9, 2
z := mydiv(x, y)
```
Ответ: <code>Функция возвращает результат по указателю;</code><br>
<code>В точке вызова будет получен адрес по которому лежит переменная result;</code>

- Дан фрагмент кода на языке С++. Будет ли код работать?
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}

int main(){
    print(1, 2, " ");
}
```
Ответ: <code>Да. Ошибок нет;</code>

- Дана функция на языке С++. Выберите все варианты вызова данной функции, при которых произойдёт обмен значениями переменных x и y. Переменные объявлены следующим образом: int x = 1; и int y = 2;:
```cpp
void swap(int a, int b){
    int t = a;
    a = b;
    b = t;
}
```
Ответ: <code>Эта функция не может выполнить требуемое действие;</code>

- Язык Go. Функция div должна вернуть вернуть 2 значения. Выберите все допустимые сигнатуры:<br>

Ответ: <code>func div(a, b float64) (float64, error)</code><br>
<code>func div(a, b float64) (res float64, err error)</code>

- Дана функция на языке С++. Выберите всё варианты, которые являются определением этой функции:
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```
Ответ:
```cpp
void print(short a, short b, std::string sep){
    std::cout << a << sep << b;
}
```

- Дана функция на языке С++. Выберите все верные утверждения:
```cpp
int* mydiv(int a, int b){
    int result = a % b;
    return &result;
}
```
При условии, что функция вызывается так:
```cpp
int x = 9, y = 2;
int* z = mydiv(x, y);
```
Ответ: <code>В точке вызова будет получен адрес по которому лежала переменной result во время работы функции mydiv;</code><br>
<code>Функция возвращает результат по указателю;</code>

- Язык С++. Выберите прототипы функций, для которых обязательно наличие оператора return в теле:<br>

Ответ:
```cpp
std::string& strip(std::string& src);
```
```cpp
double next();
```
```cpp
int sum(int a, int b);
```


- Дана функция на языке С++. Выберите все верные утверждения:
```cpp
int min(int* a, int* b){
    return *a < *b ? *a : *b;
}
```
При условии, что функция вызывается так:
```cpp
int x = 10, y = 0;
min(&x, &y);
```
Ответ: <code>Параметры функции получают адреса, по которым расположены переменные;</code><br>
<codeФункция принимает аргументы по указателю;</code>

- Код на языке Go. Выберите все позиции (отмеченные комментарием) в которых можно определить функцию sum.
```go
// 1
package main
// 2
import "fmt"
// 3
func main() {
    // 4
    fmt.Println("Hello World")
    // 5
}
// 6
```
Ответ: <code>6 3</code><br>
