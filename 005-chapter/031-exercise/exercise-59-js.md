

### Формулировка
Создать программу, которая перемешивает элементы массива в случайном порядке.

### Пояснение
Программа должна принимать на вход массив и перемешивать его элементы так, чтобы порядок элементов был случайным.

### Тесты

1. **Пример 1:**
   - Вход: [1, 2, 3, 4, 5]
   - Ожидаемый результат: Массив, содержащий те же элементы, что и входной массив, но в случайном порядке.

2. **Пример 2:**
   - Вход: [-10, 0, 10, -5, 7]
   - Ожидаемый результат: Массив, содержащий те же элементы, что и входной массив, но в случайном порядке.

3. **Пример 3:**
   - Вход: [5, 5, 5, 5, 5]
   - Ожидаемый результат: Массив, содержащий те же элементы, что и входной массив, но в случайном порядке.

### JavaScript
```javascript
function shuffleArray(arr) {
    for (let i = arr.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [arr[i], arr[j]] = [arr[j], arr[i]];
    }
    return arr;
}

// Пример использования
console.log("Пример 1:", shuffleArray([1, 2, 3, 4, 5]));
console.log("Пример 2:", shuffleArray([-10, 0, 10, -5, 7]));
console.log("Пример 3:", shuffleArray([5, 5, 5, 5, 5]));
```

