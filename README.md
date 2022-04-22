---
version: '3.8'
services:
 db:
  image: mysql
  environment:
   MYSQL_ROOT_PASSWORD= intelliqit
 wordpress:
  image: wordpress
  ports:
   - 8888:80
  deploy: 
   replicas: 4
