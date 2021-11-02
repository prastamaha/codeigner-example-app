# Simple Blog with Codeigniter 3
Simple blog with codeigniter3 to practice CRUD functionality. This will help you up and running with codeigniter3.

source repo: [https://github.com/ashiqulislam/CodeIgniter-3-blog](https://github.com/ashiqulislam/CodeIgniter-3-blog)

## Features
1. Cusom route.
2. Blog post with image upload.
3. Blog comment.
4. Category for blog post.
5. User registration and Login.

## Installation
- gic clone or donwload the zip file.
- Extract zip file
- Upload db.sql on phpmyadmin.
- Configure the confg/database.php file.
- Configure the base_url on confg/confg.php 

## Docker Installation
- setup .env file variable
- running aplication

using php-fpm
```
docker-compose -f docker-compose-fpm.yml up --build
```

using php-apache
```
docker-compose -f docker-compose-apache.yml up --build
```
