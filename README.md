# test_byu_product_onlinetradeshop

Тест покупки выбранного товара после использования группы фильтров без регистрации на сайте. Онлайн магазин https://www.onlinetrade.ru/
Настройки браузера в файлe conftest.py. 
Добавлено логирование и отчеты в allure
Запуск теста pysarm:
  py.test --alluredir=%allure_result_folder% ./tests
  allure serve %allure_result_folder%


Тест кейс.
  ШАГИ
1. Зайти на сайт https://www.onlinetrade.ru/
2. Нажать на каталог
3. Кликнуть на категорию "Зоотовары"
4. Кликнуть на блок "Для собак"
5. Кликнуть на блок "Корм для собак"
6. Выбрать фильтры:
   - в наличии
   - сухой
   - ягненок
   - корм Brit
7. Указать вес упаковки корма 15 кг
9. Нажать на кнопку "Подобрать"
10. Нажать кнопку "Купить"
11. Кликнуть по кнопке "Оформить заказ"
    ОР
    В корзине отображатеся выбранный товар

