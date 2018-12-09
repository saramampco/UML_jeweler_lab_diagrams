# Описание интерфейса IPayment
Интерфейс предназначен для работы с методами класса Payment

## Реализация интерфейса
* **Add**(PaymentID : Int): Int – функция, добавляющая платёж в базу данных;
* **Del**(PaymentID : Int) : Bool – функция, удаляющая платёж из программы;
* **FindAll**(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List<[Payment](https://github.com/saramampco/oop/blob/master/docs/Payment.md)> – функция, возвращающая список платежей с заданными параметрами. Параметры:
	
	*sortintg : string — отвечает, по какому полю будет сортироваться список;
	
	*filtering : string — отвечает за фильтрацию;
	
	*sortingA : boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	
	*count : int — отвечает, сколько элементов необходимо показать;
	
	*page : int — отвечает, с какой страницы начинать поиск элементов;
	
* **FindByID**(ID : Int) : [Payment](https://github.com/saramampco/oop/blob/master/docs/Payment.md) – функция, осуществляющая поиск платежа в базе данных по ID и возвращающая найденный, если такой есть;
* **Save**(Payment: [Payment](https://github.com/saramampco/oop/blob/master/docs/Payment.md)) : Bool – функция, редактирующая данные о платеже. Параметр «Payment» — платёж, которого необходимо редактировать в БД.
