## Раздел 1: Введение

### 1-2. Что такое React
  - Open Source UI библиотека
  - JSX
  - Использует UI компоненты
  - Использует reconciliation алгоритм
  
---
### 1-3. Первое react приложение
[https://codesandbox.io/](https://codesandbox.io/)

---
### 1-4. Среда разработки

    npm i -g create-react-app
    mkdir react-apps
    cd react-apps/
    create-react-app todo
    cd todo
    ls
    npm start
    
    
## Раздел 2: ECMAScript 2019

### 2-1. let и const

* **let**  - переменная
* **const**  - константы
* область видимости блок кода {}

Используй **const**. Если действительно нужно поменять значение, то **let** 

### 2-2. Arrow-функции

* const f = (x) => x * x;
* cохраняет лексическое значение this
* нет свойства .prototype, не могут быть вызваны с new

### 2-3. Параметры по-умолчанию

* const f = (a = 10, b = true) => {};
* устанавливается если не передается значение или передается undefined
* могут иметь любой тип