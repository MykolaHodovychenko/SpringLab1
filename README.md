# Лабораторна робота 1. Розробка простого RESTful веб-сервісу за допомогою фреймворку Java Spring

### Задачі:

1. Створити класи сутностей відповідно до завдання
2. Створити класи сервісів, в яких передбачити списки для об'єктів класів сутностей
3. В конструкторах сервісів передбачити початкові дані для списків, якщо це потрібно виходячи із завдання
4. В класах сутностей передбачити методи для управління об'єктами сутностей в списках
5. Розробити один або декілька класів REST-контролерів
6. Створити методи для обробки запитів відповідно до завдання
7. Завантажити, встановили та зареєструватися в додатку Postman
8. Створити нову колекцію запитів
9. Створити запити відповідно до варіанту завдання
10. Запустити серверний додаток
11. Переконатися, що всі запити, створені у Postman, працюють коректно та повертають коректний результат
12. Експортувати колекцію запитів в формат JSON та додати до цього програмного проєкту

**Варіант завдання обирається відповідно до списку групи, який надає староста групи**

**Variant 1: E-commerce Platform**

Topic: Develop a RESTful web service for an e-commerce platform.

Entities:

- Product: id, name, description, price, quantity.
- Customer: id, name, email, address.
- Order: id, customer_id, product_id, quantity, total_price, status.

Queries to Server:

1. Add a new product.
2. Retrieve product details by ID.
3. Update product information.
4. Delete a product.
5. Register a new customer.
6. Get customer details by ID.
7. Update customer information.
8. Remove a customer.
9. Place a new order.
10. Retrieve order details by ID.

**Variant 2: Task Management System**

Topic: Build a RESTful web service for a task management system.

Entities:

- Task: id, title, description, due_date, status.
- User: id, username, email, password.
- Project: id, name, description, start_date, end_date.

Queries to Server:

1. Create a new task.
2. Get task details by ID.
3. Update task information.
4. Delete a task.
5. Register a new user.
6. Retrieve user details by ID.
7. Update user information.
8. Delete a user.
9. Create a new project.
10. Fetch project details by ID.

**Variant 3: Library Management System**

Topic: Develop a RESTful web service for a library management system.

Entities:

- Book: id, title, author, ISBN, genre.
- Member: id, name, email, phone.
- Loan: id, book_id, member_id, issue_date, return_date.

Queries to Server:
1. Add a new book.
2. Retrieve book details by ID.
3. Update book information.
4. Remove a book.
5. Register a new member.
6. Get member details by ID.
7. Update member information.
8. Remove a member.
9. Issue a book to a member.
10. Retrieve loan details by ID.

**Variant 4: Social Media Platform**

Topic: Create a RESTful web service for a social media platform.

Entities:

- User: id, username, email, password.
- Post: id, content, author_id, timestamp.
- Comment: id, post_id, content, author_id, timestamp.

Queries to Server:

1. Register a new user.
2. Fetch user details by ID.
3. Update user information.
4. Delete a user.
5. Create a new post.
6. Retrieve post details by ID.
7. Update post content.
8. Delete a post.
9. Add a comment to a post.
10. Get comment details by ID.

**Variant 5: Healthcare Appointment System**

Topic: Develop a RESTful web service for managing healthcare appointments.

Entities:

- Doctor: id, name, specialization, email, phone.
- Patient: id, name, gender, date_of_birth, email, phone.
- Appointment: id, doctor_id, patient_id, date_time, status.

Queries to Server:

1. Add a new doctor.
2. Retrieve doctor details by ID.
3. Update doctor information.
4. Remove a doctor.
5. Register a new patient.
6. Get patient details by ID.
7. Update patient information.
8. Delete a patient.
9. Schedule a new appointment.
10. Retrieve appointment details by ID.

**Variant 6: Recipe Sharing Platform**

Topic: Develop a RESTful web service for a recipe sharing platform.

Entities:

- Recipe: id, name, description, ingredients, instructions.
- Chef: id, name, specialization, location.
- Review: id, recipe_id, reviewer_id, rating, comment.

Queries to Server:
1. Add a new recipe.
2. Retrieve recipe details by ID.
3. Update recipe information.
4. Delete a recipe.
5. Register a new chef.
6. Get chef details by ID.
7. Update chef information.
8. Delete a chef.
9. Add a review to a recipe.
10. Get review details by ID.

**Variant 7: Job Posting Platform**

Topic: Create a RESTful web service for a job posting platform.

Entities:

- Job: id, title, description, location, salary.
- Employer: id, name, industry, location.
- Application: id, job_id, applicant_id, status, date_applied.

Queries to Server:

1. Post a new job.
2. Retrieve job details by ID.
3. Update job information.
4. Remove a job.
5. Register a new employer.
6. Get employer details by ID.
7. Update employer information.
8. Delete an employer.
9. Submit an application for a job.
10. Fetch application details by ID.

**Variant 8: Online Learning Platform**

Topic: Build a RESTful web service for an online learning platform.

Entities:

- Course: id, title, description, instructor, price.
- Student: id, name, email, enrolled_courses.
- Enrollment: id, course_id, student_id, enrollment_date.

Queries to Server:
1. Publish a new course.
2. Retrieve course details by ID.
3. Update course information.
4. Remove a course.
5. Register a new student.
6. Get student details by ID.
7. Update student information.
8. Delete a student profile.
9. Enroll a student in a course.
10. Fetch enrollment details by ID.

**Variant 9: Car Rental System**

Topic: Develop a RESTful web service for managing car rentals.

Entities:

- Car: id, make, model, year, price_per_day, available.
- Customer: id, name, email, contact_number.
- Rental: id, car_id, customer_id, rental_start_date, rental_end_date, total_cost.

Queries to Server:

1. Add a new car to the rental fleet.
2. Retrieve car details by ID.
3. Update car information.
4. Remove a car from the rental fleet.
5. Register a new customer.
6. Get customer details by ID.
7. Update customer information.
8. Delete a customer profile.
9. Rent a car.
10. Fetch rental details by ID.

**Variant 10: Hotel Reservation System**

Topic: Build a RESTful web service for hotel room reservations.

Entities:

- Room: id, room_number, type, price_per_night, available.
- Guest: id, name, email, phone, address.
- Reservation: id, guest_id, room_id, check_in_date, check_out_date, total_cost.

Queries to Server:
1. Add a new room.
2. Retrieve room details by ID.
3. Update room information.
4. Remove a room.
5. Register a new guest.
6. Get guest details by ID.
7. Update guest information.
8. Delete a guest profile.
9. Make a reservation.
10. Fetch reservation details by ID.