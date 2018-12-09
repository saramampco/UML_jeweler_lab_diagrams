# Описание интерфейса IOrder
Интерфейс предназначен для работы с методами класса Order

## Реализация интерфейса
* Add(OrderID : Int) : Int  – функция, добавляющая заказ в базу данных;
* AddMaterialAmount(OrderID : Int, MaterialID : Int, Amount : Double) : bool – функция, добавляющая количество материала к заказу.  Параметры OrderID и MaterialID – ID по которому будет осуществлен поиск в базе. Amount – количество добавленного материала;
* Del(OrderID : Int) : Bool – функция, удаляющая заказ из программы;
* DelMaterialAmount(OrderID : Int, MaterialID : Int, Amount: Double) : Bool – функция, удаляющая из заказа количество материала;
* FindAll(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List<[Order](https://github.com/saramampco/oop/blob/master/docs/Order.md)> – функция, возвращающая список заказов с заданными параметрами. Параметры: 
    sortintg: string — отвечает, по какому полю будет сортироваться список;
    filtering: string — отвечает за фильтрацию;
    sortingA: boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
    count: int — отвечает, сколько элементов необходимо показать;
    page: int — отвечает, с какой страницы начинать поиск элементов;
* FindByID(ID : Int) : [Order](https://github.com/saramampco/oop/blob/master/docs/Order.md) – функция, осуществляющая поиск заказа в базе данных по ID и возвращающая найденный, если такой есть;
* GetOrderMaterials(OrderID : Int) : Dictionary< [Material](https://github.com/saramampco/oop/blob/master/docs/Material.md), Double> – функция, возвращающая коллекцию с материалами, использованными в заказе, и их количество;
* getTotalCost(OrderID : Int) : double – функция, возвращающая итоговую стоимость заказа;
* Save(Order : Order) : Bool – функция, редактирующая данные о заказе. Параметр «Order» — заказ, который необходимо редактировать в БД
