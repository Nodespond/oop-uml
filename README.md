Предметная область моей диаграммы - таксомоторная фирма(таксопарк)
Таксопарк содержит 7 основных аспектов(сущностей) . К ним относятся: компания(Company), машины(Car),заказы(Order),механики(Mechanic),диспетчера(Dispatcher),водители(Driver).Поверх диспетчеров, водителей и механиков стоит класс людей (Human).

Компания содержит имя (Name) , юридический адрес(Adress) и имеет автопарк(Autopark).Она может увеличивать штат водителей (addDriver(driver : Driver) ) или количество машин в парке (addCar(car: Car) ).

Водители, диспетчера и механики наследуют атрибуты имени(Name) и возраста (Age) от класса Human и являются членами компании(Company).

Водитель имеет свой рейтинг (Rating). Он может узнать его (GetRating() : Integer). Также он может взять заказ (GaveOrder (order : Order)) или машину (GetCar(car : Car)).Он управляет машиной.

Диспетчер обладает должностью (Post) и занимается созданием (createOrder(info : info): Order) , отменой (removeOrder(order: Order) ) и изменением заказов (ChangeInfo(order: Order)).

Механик занимается диагностикой ( checkCar(car : Car) ) и починкой автомобилей ( repareCar(car: Car)).

Заказ содержит в себе информацию(Info), стоимость (Cost) и прибавку в рейтинге (RatingUp).

Машина содержит название модели (Model), класс( СarClass) и статус состояния (Status). Можно проверить статус машины( checkStatus(): String) и прикрепить к ней водителя (GetDriver (driver : Driver) ) .
![diagram](https://github.com/Nodespond/oop-uml/assets/145635207/d470b35a-d662-49a0-a07f-8d7f69ccbc53)

