# Отчёт о тестировании Приема платежей с банковских карт организациям

## Краткое описание

29.06.21. - 29.06.21. было проведено функциональное тестирование валидации номера банковской карты приложения <Прием платежей с банковских карт организациям>.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:
* https://github.com/VladimirAlf/CreditCart/issues/1#issue-935473016
* https://github.com/VladimirAlf/CreditCart/issues/2#issue-935555745


## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* Код src/Main.java (открыв commit проскролить ниже .gitignore) 2f3646dbb3526031a363303c671c047f1c1f66b7
* freeformatter.com - сайт генерации валидных номеров кредитных карт


В качестве тестовых данных использовались данные c freeformatter.com - для генерации валидных номеров кредитных карт:
* Валидная карта из 16 цифр проходит валидацию. Скриншот https://monosnap.com/file/7o8iotMeQ9fs9AllqiYPNJdqd2IeaS
* Валидная карта из 19 цифр не проходит валидацию. Скриншот https://monosnap.com/file/RScdxwOECjJy7pHmcQMpfOMy9lvmuD
* Валидная карта из 16 цифр проходит валидацию. Скриншот https://monosnap.com/file/QzaTT3ZEv5GnLbe4hj8CXHMmYmkzLt
* Валидная карта из 19 цифр не проходит валидацию. Скриншот https://monosnap.com/file/zHSnYvMfI4YUwbiJq2Uit3zt5kIRMq

Тестирование производилось в следующем окружении:
* Windows 10 Home, 64-разрядная ОС
* OpenJDK11U-jdk_x64_windows_hotspot_11.0.11_9
* Intellij IDEA Community Edition 2021.1.2