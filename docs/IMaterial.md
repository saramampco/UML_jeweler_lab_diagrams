# Описание интерфейса IMaterial
Интерфейс предназначен для работы с методами класса Material

## Реализация интерфейса
* **Add**(MaterialID : Int): Int – функция, добавляющая материал в базу данных;
* **Del**(MaterialID : Int) : Bool – функция, удаляющая материал из программы;
* **FindAll**(sorting : string, filtering : string, sortingA : boolean, count : int, page : int) : List<[Material](https://github.com/saramampco/oop/blob/master/docs/Material.md)> – функция, возвращающая список материалов с заданными параметрами. Параметры:
    
	*sortintg : string — отвечает, по какому полю будет сортироваться список;
	
	*filtering : string — отвечает за фильтрацию;
	
	*sortingA : boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
	
	*count : int — отвечает, сколько элементов необходимо показать;
	
	*page : int — отвечает, с какой страницы начинать поиск элементов;
	
* **FindByID**(ID : Int) : [Material](https://github.com/saramampco/oop/blob/master/docs/Material.md) – функция, осуществляющая поиск материала в базе данных по ID и возвращающая найденный, если такой есть;
* **GetRemnantInSubmittals**(MaterialID : Int) : Dictionary<[Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal.md), double> – функция, возвращающая остатки материалов в филиалах с их количеством;
* **Save**(Material : [Material](https://github.com/saramampco/oop/blob/master/docs/Material.md)) : Bool – функция, редактирующая данные о материале. Параметр «Material» — материал, которого необходимо редактировать в БД.
