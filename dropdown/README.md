# Выпадающие списки

Домашнее задание к занятию 1.3 «Объект события».

## Описание 

Необходимо создать управление кнопкой с прикреплённым к ней выпадающим списком

![Demo](./demo.gif)

### Исходные данные

1. Основная HTML-разметка
2. Базовая CSS-разметка

Базовая разметка кнопки представлена следующим кодом:

```html
<div class="dropdown">
    <div class="dropdown__value">JavaScript</div>
    <ul class="dropdown__list">
        <li class="dropdown__item">
            <a href="" class="dropdown__link">
                JavaScript
            </a>
        </li>
        <li class="dropdown__item">
            <a href="" class="dropdown__link">
                PHP
            </a>
        </li>
        <li class="dropdown__item">
            <a href="" class="dropdown__link">
                Python
            </a>
        </li>
        <li class="dropdown__item">
            <a href="" class="dropdown__link">
                Fortran
            </a>
        </li>
    </ul>
</div>
```

В элементе с классом *dropdown__value* содержится выбранное значение.

Для того, чтобы открыть меню, требуется проставить класс *dropdown__list_active*:

```html
<ul class="dropdown__list dropdown__list_active"></ul>
```

Нажатие на элемент с классом *dropdown__item* при открытом списке должно:
1. Закрывать список
2. Устанавливать новое значение в элемент с классом *dropdown__value*
