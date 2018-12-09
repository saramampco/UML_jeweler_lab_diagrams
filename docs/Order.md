# Описание класса Order
Класс для работы с заказами

## Атрибуты

* ID: Int
* Client: List<[Client](https://github.com/saramampco/oop/blob/master/docs/Client "Объект класса Client")>
* Jeweller: List<[Jeweller](https://github.com/saramampco/oop/blob/master/docs/Jeweller "Объект класса Jeweller")>
* StartDate: DateTime
* EndDate: DateTime
* Prepayment: Double
* ProductType: String
* Submittal: List<[Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal "Объект класса Submittal")>
* TotalCost: Double
* TotalProductWeight: Double
* WorkCost: Double
* State: Bool

## Описание атрибутов

* ID: Int - идентификатор в БД
* Client: List<[Client](https://github.com/saramampco/oop/blob/master/docs/Client "Объект класса Client")> - список клиентов
* Jeweller: List<[Jeweller](https://github.com/saramampco/oop/blob/master/docs/Jeweller "Объект класса Jeweller")> - список ювелиров
* StartDate: DateTime - дата создания заказа
* EndDate: DateTime - дата завершения заказа
* Prepayment: Double - предоплата
* ProductType: String - тип изделия
* Submittal: List<[Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal "Объект класса Submittal")> - список филиалов
* TotalCost: Double - итоговая стоимость
* TotalProductWeight: Double - итоговый вес изделия
* WorkCost: Double - стоимость работы
* State: Bool - статус заказа
