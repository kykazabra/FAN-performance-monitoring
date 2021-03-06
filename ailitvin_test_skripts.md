# Литвин Андрей - "Инструмент тестирования и оценки эффективности системы охлаждения CPU в ПК."

### Группа: 10 - МИ - 2
### Электронная почта: kykazabra@gmail.com
### VK: www.vk.com/tcarroflan


## Функционал проекта
Инструмент тестирования и оценки эффективности системы охлаждения CPU в ПК. (Разработка приложения Cooler Tester)

## Процесс тестирования при разработке
В процессе написания и добавления нового кода в программу, тестироваться будет как отдельный функционал новой добавленной части, так и работоспособность программы в целом.

Проект будет состоять из 3 крупных модулей:
1. Загрузки процессора
2. Сбора информации с систем мониторинга материнской платы  
3. Отображения собранных данных пользователю

Для проверки корректности работы кода, отвечающего за нагрузку процессора, я буду использовать системную утилиту Windows - Performance Monitoring.
Работу модуля сбора информации я буду оценивать, сравнивая полученные модулем результаты (при нагрузке в условной игре) с результатами коммерческой утилиты HW Monitoring pro.
Модуль UI я буду тестировать с помощью пользовательских сценариев: запуск проекта, переход по всем возможным вкладкам, отрисовка графиков и т.д. 

Общее тестирование утилиты будет произведено следующим образом. На испытуемом компьютере запускается тест, контролируется достижение процессором нагрузки в 99%, рост температуры ядер процессора, при этом отслеживается частота ядер.
 
1. В случае, если система охлаждения подобрана адекватно, относительно мощности процессора, через некоторое время должен наблюдаться баланс, при котором загрузка CPU - 99%, температура стабилизируется на определенном уровне и перестает расти, а частота ядер достигает максимально возможного значения для данного процессора. 
2. Если система охлаждения не соответствует мощности процессора, будет наблюдаться ситуация, отличная от описанной картины (рост температуры не остановится, и у процессора сработает система защиты, что будет наблюдаться, как циклическая модуляция частоты ядер). 
 
## Процесс демонстрации работы программы при сдаче
Для демонстрации программы при сдаче проекта мы берем условный компьютер, запускаем на нем утилиту и начинаем тест. Убеждаемся, что выполняется условие 1 (см. выше). Далее искусственным образом ухудшаем характеристики системы охлаждения, например, отключаем вентилятор у процессора или накрываем одеялом компьютер. Убеждаемся, что наступает случай 2. Возможен так же и случай 3 :))), когда перегреется оперативная память или материнская плата, что приведет к "синему экрану BSOD :)", что так же докажет недостаточность эффективности системы охлаждения.  
 
