# MySQL-Final-Fall-Project
Inner Join
SELECT student.first_name, student.last_name, student.score, school.name, city.name,
city.county FROM `student`
INNER JOIN class ON student.class_id=class.id
INNER JOIN room ON class.room_id = room.id
INNER JOIN school ON room.school_id = school.id
INNER JOIN city ON school.city_id = city.id
ORDER BY student.score DESC;
