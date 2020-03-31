# МРРТ контроллер заряда батареи

Контроллер заряда управляется с помощью специализированного микроконтроллера STM32F334C8T6 с высокоразрядным ШИМ-контроллером (HRPWM) на борту. Применение данного устройства возможно, как в роли отладочного комплекса для изучения алгоритмов поиска точки максимальной мощности (ТММ), так в качестве законченного устройства для работы в автономной солнечной электростанции мощностью до 500 Вт.

![Фото МРРТ](https://habrastorage.org/webt/m9/jz/zv/m9jzzv8udvu62hfujno-cwyeerg.jpeg)

При разработке контроллера заряда основной упор делается на создание надежной аппаратной части с применением лучших компонентов и на реализацию максимально эффективных алгоритмов поиска ТММ. В контроллере отсутствую электролитические конденсаторы, вместо них примененые твердотельные полимерные конденсаторы с повышенным сроком службы, а так же оптимизированы тепловые режимы работы устройства, что в комплексе позволит обеспечить гарантированный ресурс работы не менее 10 лет. Это приведет к увеличению надежности автономных мини-электростанций и снижению затрат на обслуживание оборудования.

# Технические характеристики

* Входное напряжение: *15...60В*
* Выходное напряжение: *12/24В*
* Выходной зарядный ток: *20А*
* Стабилизация тока: *±1,5%*
* Стабилизация напряжения: *±2%*
* Рабочая частота: *100кГц*
* КПД, не менее: *94%*
* Алгоритмы МРРТ: *да*
* Типы аккумуляторов: *AGM, GEL, Li-ion, LiFePo4*
* Интерфейсы: *CAN, Wi-Fi*
* Габаритные размеры: *136х70х26мм*
* Температура эксплуатации: *-40...+85<sup>o</sup>C*

# Структура проекта

* **docs** - документация на проект: ВОМ, принципиальная схема и прочее
* **hardware** - исходные проект PCB
* **manufacture** - gerber файлы для заказа ПП на производстве
* **mechanical** - исходный проект корпуса РЭА

# Печатная плата

Контроллер заряда выполнен на единой 4-х слойной печатной плате (ПП) толщиной **1,6 мм** из материала FR-4 и толщиной меди 1 Oz или 35 мкм. <font color="red">*При изменение толщины платы необходима корректировка корпуса устройства!*</font>

![Печатная плата МРРТ контроллера](https://habrastorage.org/webt/_t/5y/04/_t5y04h44n1iqy3mmhm5vbnzupa.jpeg)

# Лицензирование

Все исходные материалы для проекта распространяются по лицензии [MIT](./LICENSE "Описание лицензии"). Вы можете использовать проект в любом виде, в том числе и для коммерческой деятельности, но стоит помнить, что автор проекта не дает никаких гарантий на работоспособность устройства или частей проекта, а так же не несет никакой ответственности по искам или за нанесенный ущерб.
