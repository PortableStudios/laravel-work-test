# Portable Laravel Work Test

## About this work test
---
This repository contains a basic Laravel 9 scaffold, with Laravel Sail pre-configured to allow a basic runtime environment.  If you are not familiar with Laravel Sail, after cloning the repository, you should be able to get the environment running by executing:

`vendor/bin/sail up -d`
`vendor/bin/sail artisan migrate`

from the project root.  Your site will be available at `http://laravel.test/`, which you may need to add to your hosts file (pointing at `127.0.0.1`).  

All `artisan` commands are now executed as `vendor/bin/sail artisan`.  You may like to add an alias for `sail` to point to the vendor directory.

This README provides a step-wise series of tasks you will do together with a Portable staff member during your technical interview to demonstrate basic coding competencies and explore your problem solving process.  Don't worry if you don't get to go through all of them at interview - this set is designed to be flexible for various amounts of available time and varying levels of developer experience.

## Tasks
---
1. Add a new date field to the `User` model called `dob` which represents the user's date of birth, and a new attribute called `underage`, which returns a boolean specifying if the user is currently under 18 (true).
2. Write a unit test to verify the implementation of step 1.
3. Add a page accessible at "/users" which returns the name, date of birth and underage status of all users.
4. Write a unit test to verify the implementation of step 3.
5. Add a page accessible at "/users/create" which allows for the creation of a new user.  All fields are required, and the user must be at least 14 years old.
6. Add a unit test to verify the implementation of step 5.