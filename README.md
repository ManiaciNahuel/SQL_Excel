> https://drive.google.com/drive/u/0/folders/1_2FSaV95zTEjkW3LuzYfcdfI-HkhFrIG
> https://chat.openai.com/c/ea613bb4-9bea-4b77-a169-b737c187789b
> https://drive.google.com/drive/u/0/folders/1t_VEi0e-o5tpQO_AF9X0HkMybA1ntLy6

EXCEL

- SUMA
- CONCATENAR
- SUMAR.SI
- CONTAR
- CONTAR.SI
- BUSCARV
- PROMEDIO
- PROMEDIO.SI
- IZQUIERDA
- DERECHA
- EXTRAE
- CARACTERES COMODIN 
- ?    *   ~?*   <o>
- SI ANIDADO
- SI.CONJUNTO
- =SI.ERROR(INDICE(B4:B15;COINCIDIR(C17;C4:C15;0)); "Not found")


SQL 
> https://www.w3schools.com/sql/sql_groupby.asp
> https://www.w3schools.com/sql/sql_join.asp
> https://intellipaat.com/blog/tutorial/sql-tutorial/sql-commands-cheat-sheet/
> https://devhints.io/mysql

- SELECT * FROM Customers;
- SELECT CustomerID FROM Customers ;
- SELECT CustomerID as CustomerID, City, Counttry FROM Customers;
- SELECT ContactName FROM Customers WHERE CustomerID < 3;
- SELECT ContactName as CustomerID, City FROM Customers WHERE CustomerID < 3; 
- SELECT CustomerID FROM Customers WHERE ContactName IS NULL;
- 
- SELECT ContactName FROM Customers WHERE ContactName LIKE ... 
- ... 'a%';  //Empieza con a
- ...  '%a'; //Termina con a
- ...  'a%a'; //Empieza y termina con a
- ...  '%aria%'; //Contiene aria
- ...  '_a%'; //Tiene a en la segunda posicion 
- ...  '___a%'; //Tiene a en la cuarta posicion 
- ...  'a___%'; //Empieza con a y tiene mas de 4 caracteres de lenght
- 
- SELECT columns
- FROM table1 name
- INNER JOIN table2 name
- ON table1.coumn_x = table2.column_y;
- 
- SELECT *
- FROM table1
- INNER JOIN table2
- ON table1.CategoryID= table2.CategoryID
- WHERE table2.Price BETWEEN 10 AND 20;

- SELECT *
- FROM Products
- INNER JOIN Categories
- ON Products.CategoryID= Categories.CategoryID
- WHERE Products.ProductName BETWEEN 'A' AND 'F'
- AND Products.Price < 20
- ORDER BY Products.ProductName ASC;
- 
- SELECT column_name(s)
- FROM table_name
- WHERE condition
- GROUP BY column_name(s)
- ORDER BY column_name(s);

List the number of customers in each country.
- 
- SELECT COUNT(CustomerID), Country
- FROM Customers
- GROUP BY Country;

List the number of customers in each country, ordered by the country with the most customers first.

- SELECT COUNT(CustomerID), Country
- FROM Customers
- GROUP BY Country
- ORDER BY COUNT(CustomerID) DESC;