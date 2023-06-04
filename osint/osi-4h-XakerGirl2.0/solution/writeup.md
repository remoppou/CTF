# XakerGirl 2.0

|   Cобытие   | Название | Категория | Сложность |
| :---------: | :------: | :-------: | :-------: |
| VKACTF 2023 |  XakerGirl 2.0  |  Osint  |  Тяжело  |

## Описание

>Автор: Pashkevich
>
>Наша любимая девочка снова на связи. За прошедший год произошло многое... Поговаривают она стала шифроваться и после прошлого раза пришлось немного подлечиться и даказывать всей Алексеевской больнице, что она не тронулась умом и её действительно пытались найти в сети.Но это всё неважно. Мои источники доложили, что она снова вышла на связь и снова хулиганит. Опять она взялась за старое и при подготовке очередных испытаний загенерировала очередную тасочку. Некоторые, кто уже начал с ней разбираться отзываются так: Я хочу уйти в запой. Я, если честно, тоже хочу, но надо делать. Погнали разбираться! Всё, что у нас есть – ссылка на Google Drive.  Вот: https://drive.google.com/drive/folders/1UwSGhE4JvFlLe_YfIIMWqYKPeSiV4ZUc?usp=drive_link


# Решение

- На диске нас ждёт две картинки: Первая часть флага и картинка места. Сохраняем *_001 себе и ищём место со второй картинки.
- Отзыв отобразится, только если изменить регион, но мы то шарим за движения осинтерские...
- Нам нужен инструмент GHunt.
- Ищем инфу по почте так: ```ghunt email jamesfletcher2695@gmail.com```
- Отобразится ссылка на отзывы в GoogleMaps с второй частью флага и упоминание в календаре про Pinterest.
- Ник соответсвует почте, поэтому ссылка выглядит так ```https://pinterest.com/jamesfletcher2695/```
- В созданных пинах будет ещё 3 части флага и в описании профиля ```aHR0cHM6Ly9kcm9wbWVmaWxlcy5jb20vSDVxSlo=``` – ничто иное, как base64 ссылка на финальный кусок.
- Соединяем картинку воедино и успех достигнут. Поздравляю, Вы прекрасны!

### Флаг

Получаем наш флаг
```
vka{051N71N6_6M411_15_C001_0R_N07}
```