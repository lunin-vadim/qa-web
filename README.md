## Тестовое задание по написанию автотестов на примере корзины интернет-магазина [Магазин блокнотов](https://enotes.pointschool.ru/login)
На этапе анализа была проведена функциональная декомпозиция корзины интернет-магазина (рис. 1).
![рис. 1](/pict/1.png "рис. 1")
Основной функцией корзины является переход в нее для дальнейшего оформления заказа. Тест-кейсы  построены таким образом, чтобы протестировать работу кнопки "Переход в корзину" на всех граничных значениях, при этом с проверкой фактического результата каждого шага воспроизведения, для того, чтобы одновременно протестировать все другие функции корзины.
## Авторизация:
- **Логин**: `test`
- **Пароль**: `test`

### Тест-кейс 1. Переход в пустую корзину.
#### Предусловие: 
- Корзина пуста

| **Шаги воспроизведения** | **Ожидаемый результат** |
|----|----|
| Кликнуть на иконку корзины | Всплывает окно корзины |
| В окне корзины нажать кнопку `Перейти в корзину` | Переход на страницу корзины с возможностью дальнейшего оформления заказа) |
### Тест-кейс 2. Переход в корзину с 1 неакционным товаром.
#### Предусловие: 
- Корзина пуста

| **Шаги воспроизведения** | **Ожидаемый результат** |
|----|----|
| Добавить в корзину один товар без скидки| Рядом с корзиной отображается цифра 1 |
| Нажать на иконку корзины | Открывается окно корзины, в котором указана цена, наименование товара, общая сумма |
| В окне корзины нажать кнопку перейти в корзину| Переход на страницу корзины с возможностью дальнейшего оформления заказа)|
### Тест-кейс 3. Переход в корзину с 1 акционным товаром.
#### Предусловие: 
- Корзина пуста

| **Шаги воспроизведения** | **Ожидаемый результат** |
|----|----|
| Добавить в корзину один товар со скидкой | Рядом с корзиной отображается цифра 1 |
| Нажать на иконку корзины | Открывается окно корзины, в котором указана цена, наименование товара, общая сумма |
| В окне корзины нажать кнопку перейти в корзину| Переход на страницу корзины с возможностью дальнейшего оформления заказа)|
### Тест-кейс 4. Переход в корзину с 9 разными товарами. 
#### Предусловие: 
- Корзине 1 акционный товар

| **Шаги воспроизведения** | **Ожидаемый результат** |
|----|----|
| Добавить в корзину ещё 8 разных товаров | Рядом с иконкой корзины отображается цифра 9 |
| Нажать на иконку корзины | Открывается окно корзины, в котором указана цена, наименование товара, общая сумма |
| В окне корзины нажать кнопку перейти в корзину | Переход на страницу корзины с возможностью дальнейшего оформления заказа)|
### Тест-кейс 5. Переход в корзину с 9 акционными товарами одного наименования.
#### Предусловие: 
- Корзина пуста

| **Шаги воспроизведения** | **Ожидаемый результат** |
|----|----|
| Добавить в корзину 9 товаров одного наименования со скидкой | Рядом с иконкой корзины отображается цифра 9 |
| Нажать на иконку корзины | Открывается окно корзины, в котором указана цена, наименование товара, общая сумма |
| В окне корзины нажать кнопку перейти в корзину | Переход на страницу корзины с возможностью дальнейшего оформления заказа)|