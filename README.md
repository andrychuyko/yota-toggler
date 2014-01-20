yota-toggler
============

Простейший скрипт для переключения Yota между минимальным и обычным (выбранным
пользователем) тарифом - для попытки минимизации затрат путем перехода на
бесплатный тариф в ночное время, например.

Использование:

1. Создать в директории со скриптом файл `settings.ini`, в котором указать:

    ```bash
    LOGIN="логин"
    PASSWORD="пароль"
    OFFER_MIN="идентификатор минимального тарифа"
    OFFER_NORM="идентификатор обычного тарифа"
    ```

   Идентификаторы тарифов можно подсмотреть в средствах разработчика в
   каком-нибудь браузере при смене тарифа в личном кабинете. Это POST-запрос на
   `changeOffer`, поле `offerCode`.

2. Вызвать `yota-toggler` для включения обычного тарифа или `yota-toggler min`
   для включения минимального
