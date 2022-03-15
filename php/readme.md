1. Launch XAMPP server from Terminal
```bash
$ sudo /opt/lampp/lampp start
```
2. XAMPP directory
```bash
$ cd /opt/xampp
```
3. localhost `www.localhost/`
4. Document root folder to create PHP applications 
```bash
$ cd /opt/lampp/htdocs
```
5. Create php application `$ sudo nano NameOfApplication.php`
6. Running the application `www.localhost/MyFirstPHPApplication.php`


## PHP MYSQLi

### procedural
1. mysqli_connect() : top open a new connection. Returns an object representing the connection
2. mysqli_connect("localhost","root",,"database_name") <-  mysqli_connect(host_name, user_name, password, db_name);
3. mysqli_connect_error() - function returns error description from last connection error, and NULL if no error.
