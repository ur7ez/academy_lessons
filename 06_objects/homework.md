1. Сделайте класс `Task1`, в котором будут следующие `public` поля - `name` (имя), `age` (возраст), `salary` (зарплата).
   
   Создайте объект этого класса, затем установите поля в следующие значения (не в `__construct`, а для созданного объекта) - имя 'Иван', возраст 25, зарплата 1000. Создайте второй объект этого класса, установите поля в следующие значения - имя 'Вася', возраст 26, зарплата 2000.
   
   Выведите на экран сумму зарплат Ивана и Васи. Выведите на экран сумму возрастов Ивана и Васи.
   
2. Сделайте класс `Task2`, в котором будут следующие `private` поля - `name` (имя), `age` (возраст), `salary` (зарплата) и следующие public методы `setName`, `getName`, `setAge`, `getAge`, `setSalary`, `getSalary`.
   
   Создайте 2 объекта этого класса: 'Иван', возраст 25, зарплата 1000 и 'Вася', возраст 26, зарплата 2000.
   
   Выведите на экран сумму зарплат Ивана и Васи. Выведите на экран сумму возрастов Ивана и Васи.
   
3. Дополните класс `Task2` из предыдущей задачи `private` методом `checkAge`, который будет проверять возраст на корректность (от 1 до 100 лет). Этот метод должен использовать метод `setAge` перед установкой нового возраста (если возраст не корректный - он не должен меняться)

4. Сделайте класс `Task4`, в котором будут следующие `private` поля - name (имя), `salary` (зарплата). Сделайте так, чтобы эти свойства заполнялись в методе `__construct` при создании объекта (вот так: `new Worker(имя, возраст)` ). Сделайте также `public` методы `getName`, `getSalary`.
   
   Создайте объект этого класса 'Дима', возраст 25, зарплата 1000. Выведите на экран произведение его возраста и зарплаты.
   
5.  Сделайте класс `User`, в котором будут следующие protected поля - `name` (имя), `age` (возраст), `public` методы `setName`, `getName`, `setAge`, `getAge`.
   
   Сделайте класс `Worker`, который наследует от класса `User` и вносит дополнительное `private` поле `salary` (зарплата), а также методы `public` `getSalary` и `setSalary`.
   
   Создайте объект этого класса 'Иван', возраст 25, зарплата 1000. Создайте второй объект этого класса 'Вася', возраст 26, зарплата 2000. Найдите сумму зарплата Ивана и Васи.
   
   Сделайте класс `Student`, который наследует от класса `User` и вносит дополнительные private поля стипендия, курс, а также геттеры и сеттеры для них.
   
6. Сделайте класс `Driver` (Водитель), который будет наследоваться от класса `Worker` из предыдущей задачи. Этот метод должен вносить следующие `private` поля: водительский стаж, категория вождения (A, B, C).

7. Создайте класс `Form` - оболочку для создания форм. Он должен иметь методы `input`, `submit`, `password`, `textarea`, `open`, `close`. Каждый метод принимает массив атрибутов.
   ```
   
   	echo $form->open(['action'=>'index.php', 'method'=>'POST']);
   	//Код выше выведет <form action="index.php" method="POST">
   	
   	echo $form->input(['type'=>'text', 'value'=>'!!!']);
   	//Код выше выведет <input type="text" value="!!!">
   
   	echo $form->password(['value'=>'!!!']);
   	//Код выше выведет <input type="password" value="!!!">
   
   	echo $form->submit(['value'=>'go']);
   	//Код выше выведет <input type="submit" value="go">
   
   	echo $form->textarea(['placeholder'=>'123', 'value'=>'!!!']);
   	//Код выше выведет <textarea placeholder="123">!!!</textarea>
   
   	echo $form->close();
   	//Код выше выведет </form>
   ```
8. Создайте класс `Cookie` - оболочку над работой с куками. Класс должен иметь следующие методы: установка куки `set(имя куки, ее значение)`, получение куки `get(имя куки)`, удаление куки `del(имя куки)`.
9. Создайте класс `Session` - оболочку над сессиями. Он должен иметь следующие методы: создать переменную сессии, получить переменную, удалить переменную сессии, проверить наличие переменной сессии. Сессия должна стартовать (`session_start`) в методе `__construct`.