# Описание класса Material
Класс для работы с материалами

## Атрибуты

* ID: Int
* Name: String
* Description: String
* Order: List<[Order](https: "Объект класса Order")>
* PricePerGram: Double
* PricePerPiece: Double
* Quantity: Int
* Submittal: List<[Submittal](https: "Объект класса Submittal")>
* WeightInGrams: Double

## Описание атрибутов

* ID: Int - идентификатор в БД
* Name: String - наименование материала
* Description: String - описание материала
* Order: List<[Order](https: "Объект класса Order")> - список заказов
* PricePerGram: Double - цена за грамм
* PricePerPiece: Double - цена за штуку
* Quantity: Int - количество в штуках
* Submittal: List<[Submittal](https: "Объект класса Submittal")> - список филиалов
* WeightInGrams: Double - вес в граммах