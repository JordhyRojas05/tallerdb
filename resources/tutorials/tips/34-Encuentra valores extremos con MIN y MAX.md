### 	Encuentra valores extremos con MIN y MAX

Obtén el valor más pequeño o grande de una columna numérica o de texto.

#### Codigo
```sql
-- Crear una tabla de ejemplo
CREATE TABLE productos (
    id INT PRIMARY KEY,
    nombre VARCHAR(100),
    precio DECIMAL(10,2)
);

-- Insertar datos de ejemplo
INSERT INTO productos (id, nombre, precio) VALUES
(1, 'Laptop', 1200.99),
(2, 'Mouse', 25.50),
(3, 'Teclado', 45.99),
(4, 'Monitor', 300.00),
(5, 'Impresora', 150.75);

-- Obtener el precio más bajo
SELECT MIN(precio) AS precio_minimo FROM productos;

-- Obtener el precio más alto
SELECT MAX(precio) AS precio_maximo FROM productos;

-- Obtener el nombre alfabéticamente menor
SELECT MIN(nombre) AS nombre_primero FROM productos;

-- Obtener el nombre alfabéticamente mayor
SELECT MAX(nombre) AS nombre_ultimo FROM productos;
```
