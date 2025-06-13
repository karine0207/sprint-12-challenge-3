# sprint-12-challenge-3


Descripción

¡Hay un asesinato en SQL City!  
Este team challenge tiene como propósito tanto practicar tus habilidades en **SQL** como resolver el crimen que ha estremecido a la comunidad.  

Este proyecto fue realizado como parte del team challenge de la **Sprint 12**.

---

## 🔹 Pasos Seguidos 🔹

---
 Listado de reportes de crímenes en SQL City el 15 de enero de 2018:

sql

SELECT * FROM crime_scene_report 
WHERE date='2018-01-15' 
  AND type='murder' 
  AND city='SQL City';

Persona denominada Annabel en Franklin Ave:

SELECT * FROM person 
WHERE address_street_name='Franklin Ave' 
  AND name LIKE 'Annabel%';

 Persona en Dr. Noroeste (orden descendente por número de casa):

SELECT * FROM person 
WHERE address_street_name='Dr. Noroeste' 
ORDER BY address_number DESC;

 Entrevista de person_id = 16371:
 SELECT * FROM interview WHERE person_id='16371';

 Entrevista de person_id = 14887:
 SELECT * FROM interview WHERE person_id='14887';

 Check-ins en Get Fit Now el 9 de enero de 2018:
 SELECT * FROM get_fit_now_check_in 
WHERE check_in_date='2018-01-09' 
  AND membership_id LIKE '48Z%';

Miembros de Get Fit Now según el ID:
SELECT * FROM get_fit_now_member 
WHERE id LIKE '48Z%';

 Busca la matrícula que contenga H42W:
 SELECT * FROM drivers_license 
WHERE plate_number LIKE '%H42W%';

Persona con license_id = 423327:
SELECT * FROM person WHERE license_id='423327';

 Persona con license_id = 664760:
 SELECT * FROM person WHERE license_id='664760';

 Insertamos el nombre del culpable en la tabla solution:
 INSERT INTO solution VALUES (1, 'Jeremy Bowers');

 Verificamos que el nombre fue insertado:
 SELECT value FROM solution;
