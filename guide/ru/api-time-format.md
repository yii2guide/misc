Формат времени
===

Хранение и предоставление даты и времени основывается на международном формате **ISO 8601**.

В полях записи, которые характеризуют время работы с записью 
(добавление, редактирование и др) или действия которые происходят в настоящем 
(время аутентификации и др) должен быть тип TIMESTAMP. 
Также дата сохраняется в **+0** часовом поясе и в таком же формате отдается на запросы клиента.

Формат даты и времени:

```
<date>T<time>Z
```

* `<date>` - формат **YYYY-MM-DD**, к примеру: *2016-11-03*
* `T` - разделитель между датой и временем
* `<time>` - формат **hh:mm:ss**, к примеру: *05:22:38*
* `Z` - часовой пояс. **Z** - сокращение от *zero* имеется ввиду часовой пояс **+0** 

Полный формат:
 
 ```
 YYYY-MM-DDThh:mm:ssZ
 ```

Пример:

```
2016-11-03T05:22:38Z
```
