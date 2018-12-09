# Описание интерфейса IClient
Интерфейс предназначен для работы с методами класса Client

## Реализация интерфейса
* **Add**(ClientID : Int) : Int – функция, добавляющая клиента в базу данных;
* **AddOrder**(OrderID : Int, ClientID : Int) : Bool – функция, добавляющая заказ данному клиенту в базу данных; 
* **Del**(ClientID : Int) : Bool – функция, удаляющая клиента из программы;
* **DelOrder**(OrderID : Int, ClientID : Int) : Bool – функция, удаляющая заказ данного клиента из базы данных;
* **FindAll**(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List<[Client](https://github.com/saramampco/oop/blob/master/docs/Client.md)> – функция, возвращающая список клиентов с заданными параметрами. Параметры:
    *sortintg : string — отвечает, по какому полю будет сортироваться список;
    *filtering : string — отвечает за фильтрацию;
	*sortingA : boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	*count : int — отвечает, сколько элементов необходимо показать;
	*page : int — отвечает, с какой страницы начинать поиск элементов;
* **FindByID**(ID : Int) : [Client](https://github.com/saramampco/oop/blob/master/docs/Client.md) – функция, осуществляющая поиск клиента в базе данных по ID и возвращающая найденный, если такой есть;
* **GetAllOrders**(ClientID : Int) : List<[Order](https://github.com/saramampco/oop/blob/master/docs/Order.md)> — функция, возвращающая список заказов клиента;
* **Save(Client : [Client](https://github.com/saramampco/oop/blob/master/docs/Client.md)) : Bool – функция, редактирующая данные о клиенте. Параметр «Client» — клиент, которого необходимо редактировать в БД;
* **SaveOrder**(OrderID : Int, ClientID : Int) : Bool – функция, редактирующая данные о заказе клиента. Параметр «Order» — заказ, который необходимо редактировать в БД, Параметр «Client» — клиент, заказ которого необходимо редактировать в БД.
