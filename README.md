# Описание проекта

Интернет-магазине **«Стримчик»**, который продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, _Xbox_ или _PlayStation_).

Необходимо выявить закономерности, определяющие **успешность игры**. Это позволит сделать ставку на потенциально популярный продукт и спланировать **рекламные кампании**.

Исходные данные представляют из себя перечень игр с ключевыми характеристиками: жанр, год издания, рейтинг и т.д. Информация о количестве продаж собрана до 2016 год, включительно. Информация за 2016-ый год может быть не полной. Данные из открытых источников.

В наборе данных попадается аббревиатура [ESRB](https://www.esrb.org/) (_Entertainment Software Rating Board_) — это ассоциация, определяющая возрастной рейтинг компьютерных игр. _ESRB_ оценивает игровой контент и присваивает ему подходящую возрастную категорию, например, «Для взрослых», «Для детей младшего возраста» или «Для подростков».

## Общий вывод

Если **успех игры** исчислять количеством проданных копий, то основные параметры влияющие на объём продаж это:
- _жанр_,
- _платформа_,
- _возрастной рейтинг_,
- на их основе можно определить _территорию_ наиболее востребованных у пользователей.

Суммарно, по эти 4-ём параметрам, можно подсчитать ожидаемый диапазон продаж.

**Например**:
- `Shooter` с возрастным рейтингом `Mature`(17+) для домашних консолей `Playstation 4` - прибыльный вариант для территории **Европы**. Аналогичный вариант подойдёт **Сев. Америки**, с дополнительным каналом рекламы: `Xbox One`. Эта приставка одинакова популярна как PS4.
- `Role-Playing` или `Action` исключительно для портативной консоли `Nintendo 3DS`, возрастное ограничение ESRB не имеет значение - верный вариант для Японии.

При выборе можно учесть отзыв критиков. Желательно, чтобы оценка была от 70 баллов. Рейтинг пользователей - нельзя расценивать однозначно.

### Примечание

В перечень параметров игр можно **добавить**:
- дату релиза,
- стоимость игры (на момент выпуска),
Если эти данные уже есть, то при следующем исследовании стоит выгрузить их. Это позволит определить успех игр с финансовой стороны.