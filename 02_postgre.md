## **PostgreSQL**

Что такое транзакция? Какие у неё есть свойства?  

Транзакция объединяет последовательность действий в одну операцию и обеспечивает выполнение либо всех действий из последовательности, либо ни одного. Канонический пример — списывание денег с одного счета и зачисление на другой, что требует два update-а, которые гарантированно должны выполниться или не выполниться вместе.

Что такое уровни изолированности транзакций? Какие они бывают?  
https://ru.wikipedia.org/wiki/%D0%A3%D1%80%D0%BE%D0%B2%D0%B5%D0%BD%D1%8C_%D0%B8%D0%B7%D0%BE%D0%BB%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D0%BE%D1%81%D1%82%D0%B8_%D1%82%D1%80%D0%B0%D0%BD%D0%B7%D0%B0%D0%BA%D1%86%D0%B8%D0%B9  
Советую внимательно это прочитать, поскольку это фундаментальные вещи.  
Что такое область видимости транзакции?  
Что такое вложенные транзакции?  
Что такое курсор и зачем он нужен?  
Что делает оператор JOIN, какие виды бывают?  
Что делает оператор HAVING, примеры?  
В каких случаях вы бы предпочли нереляционную БД?  
Что такое SQL-инъекции, какие меры против?  
Что такое функциональный индекс?  
Что такое транзакиця, ее свойства?  
Какая разница между PostgreSQL и MySQL?  
Что такое VACUUM в PostgreSQL?  
Что такое проблема N + 1?

Команда VACUUM высвобождает пространство, занимаемое «мертвыми» кортежами, что актуально для часто используемых таблиц. При обычных операциях в Postgres кортежи, удаленные или устаревшие в результаты обновления, физически не удаляются, а сохраняются в таблице до очистки.

Что такое EXPLAIN? Какая разница между ним и EXPLAIN ANALYZE? 

EXPLAIN ANALYZE – в отличие от просто EXPLAIN не только показывает план выполнения запроса, но и непосредственно выполняет запрос и показывает реальное время выполнения

Что такое server side cursor и зачем он нужен?  

Способ работы с результатом запроса в базу данных, который позволяет не загружать весь объем данных в память, позволяет работать с большими объемами данных. Дополнительно углубленно можно поговорить про особенности работы в связке с pgbouncer.

Возможности PostgreSQL, отсутствующие в других БД

Источники!!!