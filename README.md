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

    const f = (x) => x * x;
* cохраняет лексическое значение this
* нет свойства .prototype, не могут быть вызваны с new

### 2-3. Параметры по-умолчанию

    const f = (a = 10, b = true) => {};
* устанавливается если не передается значение или передается undefined
* могут иметь любой тип

### 2-4. Rest параметр (собирает несколько независимых аргументов в []) 

    const f = (a, b, ...other) => {};
* всегда массив [] (может быть пустым)
* должен быть последний в списке
* максимум один rest-параметр в функции

### 2-5. Spread оператор (разворачивает массив, превращая его в список аргументов)

    const a = [1, 2];
    const max = Math.max(...a)
    const b = [...arr1, ...arr2] - *копия []*

### 2-6. Деструктуризация (Упрощает получение свойств из объектов)

    const person = {
      name: 'Sergey',
      last: 'Markov'
    }
    const { name, last, age = 18 } = person; - *Параметр по умолчанию, если сойства нет (age = 18)*
    const { name: firstname, last: lastname } = person; - *изменяет название переменных*
    
    const person = {
      name: {
        first: 'Sergey',
        last: 'Markov'
      }
    }
    const {name: {first: firstname, last: lastname} = {}} - *Получает свойства во вложенном {}*