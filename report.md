# Отчёт о тестировании установки OpenJDK
Краткое описание

18.02.2020 - 18.02.2020 были проведены:
1. Установка приложения OpenJDK в соответствии с документацией.
2. Проверка ключей с помощью приложения KeyValidator

На тестирование затрачено: 2 часа 25 минут

## В результате тестирования выявлены следующие дефекты:

1. При установке программы:
В описание указана старая версия: openjdk version "11.0.5" 2019-10-15 в результате была установлена версия openjdk version "11.0.6" 2020-01-14.

https://github.com/AlexeySuchkov/QA-KeyValidator/blob/master/Git%20CMD%20(Deprecated)%202020-02-17%2020.07.25.png

2. В процессе проверки ключей:

Из раздела "Валидные ключи" два ключи не прошли проверку и являются недействительными:

* 80b427f8-92cd-3aae-ba04-3927fbe17c6
* 387eedc6-12e9-3b32-9881-63b6b5e85317

Из раздела "Невалидные ключи" один ключ прошел проверку и оказался действительным:

* 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

https://github.com/AlexeySuchkov/QA-KeyValidator/blob/master/Bugs.png

# Описание процесса тестирования

## В процессе тестирования использовались следующие артефакты:

   * Инструкция по установке программы OpenJDK.
   * Программа KeyValidator для проверки ключей.

В качестве тестовых данных использовались данные <указать источник, откуда брались тестовые данные>:

    [Инструкция по установке OpenJDK] (https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)
    [Программа KeyValidator] (https://github.com/netology-code/javaqa-homeworks/blob/master/intro/artifacts/KeyValidator.class)
    [Руководство по использованию KeyValidator и ключи] (https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

Тестирование производилось в следующем окружении:

    Windows x64
    openjdk version "11.0.6" 2020-01-14
    
