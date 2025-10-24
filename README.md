# Задане речення
sentence = "Привіт друже, привіт світе! Це приклад речення для перевірки слова привіт."

# Розділяємо речення на слова (прибираючи розділові знаки)
import string
# Прибираємо розділові знаки
sentence_clean = sentence.translate(str.maketrans('', '', string.punctuation))

# Розбиваємо речення на слова
words = sentence_clean.split()

# Виводимо всі слова, відмінні від "привіт" (незалежно від регістру)
for word in words:
    if word.lower() != "привіт":
        print(word)
