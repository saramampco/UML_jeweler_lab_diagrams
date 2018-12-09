# Описание интерфейса ISubmittal
Интерфейс предназначен для работы с методами класса Submittal

## Реализация интерфейса
* Add(SubmittalID:Int): Int – функция, добавляющая филиал в базу данных;
* AddMaterialAmount(SubmittalID : Int, MaterialID : Int, Amount : Double) : bool - функция, добавляющая количество материала в филиал;
* Del(SubmittalID : Int) : Bool – функция, удаляющая филиал из программы;
* DelMaterialAmount(SubmittalID : Int, MaterialID : Int, Amount : Double) : Bool - удаление количества материала из филиала;
* DelSubmitalMaterial(SubmittalID : Int, MaterialID : Int) : bool - удаление материала из филиала;
* FindAll(sorting : string, filtering : string, sortingA : boolean, count : int, page : int): List<[Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal.md)> – функция, возвращающая список филиалов с заданными параметрами. Параметры: 
    *sortintg: string — отвечает, по какому полю будет сортироваться список;
    *filtering: string — отвечает за фильтрацию;
    *sortingA: boolean — отвечает, по возрастанию или убыванию будут сортироваться элементы;
    *count: int — отвечает, сколько элементов необходимо показать;
    *page: int — отвечает, с какой страницы начинать поиск элементов;
* FindByID(ID : Int) : [Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal.md) – функция, осуществляющая поиск филиала в базе данных по ID и возвращающая найденный, если такой есть;
* GetMaterialRemnant(SubmittalID : Int) : Dictionary<[Material](https://github.com/saramampco/oop/blob/master/docs/Material.md), Double> - функция, возвращающая остатки материалов в филиале;
* Save(Submittal : [Submittal](https://github.com/saramampco/oop/blob/master/docs/Submittal.md): Bool – функция, редактирующая данные о филиале. Параметр «Submittal» — филиал, который необходимо редактировать в БД.
