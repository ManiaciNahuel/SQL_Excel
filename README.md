EXCEL

SUMA
CONCATENAR
SUMAR.SI
CONTAR
CONTAR.SI
BUSCARV
PROMEDIO
PROMEDIO.SI
IZQUIERDA
DERECHA
EXTRAE
CARACTERES COMODIN 
?    *   ~?*   <o>
SI ANIDADO
SI.CONJUNTO
=SI.ERROR(INDICE(B4:B15;COINCIDIR(C17;C4:C15;0)); "Not found")


SQL 
SELECT * FROM Customers;
SELECT CustomerID FROM Customers ;
SELECT CustomerID as CustomerID, City, Counttry FROM Customers;
SELECT ContactName FROM Customers WHERE CustomerID < 3;
SELECT ContactName as CustomerID, City FROM Customers WHERE CustomerID < 3; 
SELECT CustomerID FROM Customers WHERE ContactName IS NULL;

SELECT ContactName FROM Customers WHERE ContactName LIKE ... 
... 'a%';  //Empieza con a
...  '%a'; //Termina con a
...  'a%a'; //Empieza y termina con a
...  '%aria%'; //Contiene aria
...  '_a%'; //Tiene a en la segunda posicion 
...  '___a%'; //Tiene a en la cuarta posicion 
...  'a___%'; //Empieza con a y tiene mas de 4 caracteres de lenght

SELECT columns
FROM table1 name
INNER JOIN table2 name
ON table1.coumn_x = table2.column_y;

SELECT *
FROM table1
INNER JOIN table2
ON table1.CategoryID= table2.CategoryID
WHERE table2.Price BETWEEN 10 AND 20;

FROM Products
INNER JOIN Categories
ON Products.CategoryID= Categories.CategoryID
WHERE Products.ProductName BETWEEN 'A' AND 'F'
AND Products.Price < 20
ORDER BY Products.ProductName ASC;
