--                      TASKS

--1
-- SELECT *
-- FROM categories;

--2
-- SELECT category_name, description
-- FROM categories;

--3
-- SELECT category_id as "Idlar",
--        category_name as "Nomlari",
--        description   as "Ma'lumot",
--        picture       as "Sur'ati"
-- FROM categories;

--4
-- SELECT *
-- FROM categories
-- WHERE category_name = 'Confections';

--5
-- SELECT *
-- FROM categories
-- WHERE category_name = 'Produce'
--    or category_name = 'Seafood';

--6
-- SELECT *
-- FROM categories
-- WHERE category_id between 6 and 8;

--7
-- SELECT *
-- FROM categories
-- ORDER BY description desc;

--8
-- SELECT *
-- FROM customers;

--9
-- SELECT customer_id   as "Id",
--        company_name  as "Fabrika nomlari",
--        contact_name  as "Ism familiyasi",
--        contact_title as "Lavozimi",
--        address       as "Turar joy",
--        city          as "Shahar",
--        region        as "Region",
--        postal_code   as "Shtrih kodi",
--        country       as "Davlat nomi",
--        phone         as "Telefon raqami",
--        fax           as "Pochta raqami"
-- FROM customers;

--10
-- SELECT *
-- FROM customers
-- WHERE contact_title = 'Owner';

--11
-- SELECT *
-- FROM customers
-- WHERE city = 'London';

--12
-- SELECT *
-- FROM customers
-- WHERE region IS NULL;

--13
-- SELECT *
-- FROM customers
-- WHERE region IS NOT NULL;

--14
-- SELECT *
-- FROM customers
-- WHERE country = 'Germany';

--15
-- SELECT count(country) as "Soni"
-- FROM customers
-- WHERE country = 'Germany';

--16
-- SELECT *
-- FROM customers
-- WHERE fax IS NOT NULL ORDER BY contact_name;

--17
-- SELECT *
-- FROM employees;

--18
-- SELECT employee_id       as "Id",
--        last_name         as "Familiyasi",
--        first_name        as "Ismi",
--        title             as "Lavozimi",
--        title_of_courtesy as "Taxallusi",
--        birth_date        as "Tug'ulgan sanasi",
--        hire_date         as "Boshlangan sanasi",
--        address           as "Manzili",
--        city              as "Shahar",
--        region            as "Region",
--        postal_code       as "Postal kodi",
--        country           as "Davlat",
--        home_phone        as "Uy telefon raqami",
--        extension         as "Extension",
--        photo             as "Rasm",
--        notes             as "Daftari",
--        reports_to        as "Ariza",
--        photo_path        as "Sur'ati"
-- FROM employees;

--19
-- SELECT *
-- FROM employees
-- WHERE title_of_courtesy = 'Mr.'
-- ORDER BY first_name;

--20
-- SELECT count(title)
-- FROM employees
-- WHERE title = 'Sales Representative';

--21
-- SELECT hire_date
-- FROM employees
-- WHERE hire_date BETWEEN '1994-01-01' AND '1994-12-31';

--22
-- SELECT first_name, last_name, title, city, home_phone
-- FROM employees
-- WHERE region IS NOT NULL
-- ORDER BY first_name DESC;

--23
-- SELECT *
-- FROM orders
-- WHERE customer_id = 'VINET';

--24
-- SELECT *
-- FROM orders
-- WHERE order_date between '1996-01-01' and '1996-12-31';

--25
-- SELECT *
-- FROM orders
-- WHERE ship_region IS NOT NULL;

--26
-- SELECT *
-- FROM orders
-- WHERE order_id between 10300 and 10400;

--27
-- SELECT sum(unit_price)
-- FROM order_details;
