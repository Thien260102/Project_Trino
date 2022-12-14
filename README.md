# Team:
  * Dang Ba Kien: Write some document to report
  * Vo Tan Tien: Find data for Mysql
  * Nguyen Chau Thang: Find data for PostgreSQL
  * Nguyen Van Thien (me): Leader, write report, researcher.
# Purpose of this project is run Trino in environment Docker and Ubuntu
## The first step (install some softwares):
  * Installing Java runtime environment.
  * Installing Python version 2.6x, 2.7x or 3.x.
  * Installing Mysql.
  * Installing PostgreSQL.
  * installing Trino.
## The second step (configuration):
  * Opening port of Mysql and PostgreSQL.
  * Unpacking file Trino.
  * Opening folder and create folder etc then open folder etc.
  * Create some files and write like this: 
  ![image](https://user-images.githubusercontent.com/97506616/193008875-0e01fc6e-6bc3-4464-af76-48719a84d48a.png)
  ![image](https://user-images.githubusercontent.com/97506616/193009193-06307c35-c9b4-4681-824a-fccbc57f6bd4.png)
  ![image](https://user-images.githubusercontent.com/97506616/193009301-8cecfefb-42c5-42c7-a1da-3045b7b258d0.png)
  * Then create folder catalog, open it, create some files and write like this: 
  ![image](https://user-images.githubusercontent.com/97506616/193010024-a13b4e4e-2ebc-4342-9d1b-4763b3e62721.png)
  ![image](https://user-images.githubusercontent.com/97506616/193010052-ee73b35a-a4c9-43ce-8061-fe6bda70433d.png)
  * Back to folder Trino you unpacked and create file docker-compose.yml:
  ![image](https://user-images.githubusercontent.com/97506616/193010520-00084010-f73d-4c7e-95a4-babd727823ad.png)
## The third step:
### - Opening folder contain docker-compose.yml, right mouse button, turn on terminal and running as root:
  * Run: docker-compse up
  * Displaying some infomations about containers:
  ![image](https://user-images.githubusercontent.com/97506616/193013901-dcd8b222-5eb3-4837-80ef-d46cd0e9ba31.png)
  * Then, run "docker exec -it trino_trino-coordiantor_1 trino" to starting query with TRINO

# That' all, now you can store data using Mysql and PostgreSQL and query by TRINO

# DEMO: 
 * Input: 
   + Data in Mysql: 
   ![image](https://user-images.githubusercontent.com/97506616/193016344-610427c1-e579-454a-8353-03aa31e0cea0.png)
   + Data in PostgreSQL:
   ![image](https://user-images.githubusercontent.com/97506616/193016389-b96daede-91f9-4ba2-9d3d-98dbea646a9a.png)

 * Output:
 ![image](https://user-images.githubusercontent.com/97506616/193016460-5a0de9c4-9213-4d45-ac7c-e1d8dc4ce7da.png)

