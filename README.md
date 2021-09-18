# it-oil
Исходные коды решения задания на ИТ-хакатон

Решение эмулирует идею визуализации доступности ИТ-ресурсов как основных (для головного офиса), так и в разрезе скважин. Скважины группируются по кустам и месторождениям.
В программе заложено три вида основных ресурсов: в виде "спидометра", "опрос" (периодический опрос, например, Web-сервера или сервера БД), "Лицензия" - (кол-во дней, оставшееся до истечения срока). Для каждого ресурса указывается нижнее пороговое значение, при достижении которого считается, что наступил отказ.

По скважине заложено получение двух параметров: "Есть интернет-соединение "со скважиной (Да/нет), "уровень сигнала интернет" (шкала от 0 до 5), пороговым значением принят уровень <=2. Состояние скважин определяет состояние родительских узлов дерева скважин.

Структура папок. Папка web - веб приложение на ASP.NET webapi, front-end на AngularJS (подпапка view)

Вариант развертывания: скомпилировать в Visual Studio и опубликовать приложение в папку, затем папку перенести в папку настроенного приложения в IIS. Каких-то особых настроек IIS не требуется (Аутентификация анонимная вкл, оставльные выкл.)

