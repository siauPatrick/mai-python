## issue-01
Дана функция, кодирующая строку в соответсвие с таблицей азбуки Морзе

```python
# полный код в файле morse.py
def encode(message: str) -> str:
    """
    Кодирует строку в соответсвие с таблицей азбуки Морзе
    """
    encoded_signs = [
        LETTER_TO_MORSE[letter] for letter in message
    ]

    return ' '.join(encoded_signs)
```

Напишите на неё тесты с использование `doctest`

**DoD**:
* используется директива
* используется флаг
* тест с message = 'SOS'
* тест с исклечением (Exception)
* файл README.md с описанием шагов для запуска
* файл result с командами и результатами запуска
* файл *.py с функцией и доктестами

## issue-02
Дана функция, декодирующая строку из азбуки Морзе в английский

```python
# полный код в файле morse.py
def decode(morse_message: str) -> str:
    """
    Декодирует строку из азбуки Морзе в английский
    """
    decoded_letters = [
        MORSE_TO_LETTER[letter] for letter in morse_message.split()
    ]

    return ''.join(decoded_letters)
```

Напишите на неё параметрический тест, используя `pytest.mark.parametrize`

**DoD**:
* минимум 3 тестовых примера
* файл README.md с описанием шагов для запуска
* файл result с командами и результатами запуска
* файл *.py с функцией и доктестами

