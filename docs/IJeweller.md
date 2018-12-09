# Описание интерфейса IJeweller
Интерфейс предназначен для работы с методами класса Jeweller

## Реализация интерфейса
* **Add**(JewellerID : Int) : Int – функция, добавляющая ювелира в базу данных;
* **AddOrder**(OrderID : Int, JewellerID : Int) : Bool –функция, добавляющая заказ данному ювелиру в базу данных; 
* **Del**(JewellerID : Int) : Bool – функция, удаляющая ювелира из программы;
* **DelOrder**(OrderID : Int, JewellerID : Int) : Bool – функция, удаляющая заказ данного ювелира из базы данных;
* **FindAll**(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List<[Jeweller](https://github.com/saramampco/oop/blob/master/docs/Jeweller.md)> – функция, возвращающая список ювелиров с заданными параметрами. Параметры:
   
    * sortintg : string — отвечает, по какому полю будет сортироваться список;
	
	* filtering : string — отвечает за фильтрацию;
	
	* sortingA : boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	
	* count : int — отвечает, сколько элементов необходимо показать;
	
	* page : int — отвечает, с какой страницы начинать поиск элементов;
	
* **FindByID**(ID : Int) : [Jeweller](https://github.com/saramampco/oop/blob/master/docs/Jeweller.md) – функция, осуществляющая поиск ювелира в базе данных по ID и возвращающая найденный, если такой есть;
* **GetAllOrders**(JewellerID : Int) : List<[Order](https://github.com/saramampco/oop/blob/master/docs/Order.md)> — функция, возвращающая список заказов ювелира;
* **GetAllPayments**(JewellerID : Int) : List<[Payment](https://github.com/saramampco/oop/blob/master/docs/Payment.md)> – функция, возвращающая список платежей, относящихся к ювелиру;
* **Save**(Jeweller : [Jeweller](https://github.com/saramampco/oop/blob/master/docs/Jeweller.md)) : Bool – функция, редактирующая данные о ювелире. Параметр «Jeweller» — ювелир, которого необходимо редактировать в БД;
* **SaveOrder**(OrderID : Int, JewellerID : Int) : Bool – функция, редактирующая данные о заказе ювелира. Параметр «Order» — заказ, который необходимо редактировать в БД, Параметр «Jeweller» — ювелир, заказ которого необходимо редактировать в БД.
