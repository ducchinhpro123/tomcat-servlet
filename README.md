### I named this project should_remove_1 is because I intended that this project should be removed for testing purpose.

### Instructions

Run the command below will generate the folder target/should_remove_1.war

```shell
mvn clean package 
```


Change directory to target folder

```shell
cd target/
```


Copy the generated war folder to your tomcat. It depends on your setup location.
This dir `/usr/local/tomcat9/apache-tomcat-9.0.95/webapps/` from Linux system.

```shell
cp should_remove_1.war /usr/local/tomcat9/apache-tomcat-9.0.95/webapps/
```


Change directory to /usr/local/tomcat9/apache-tomcat-9.0.95/bin
```shell
cd /usr/local/tomcat9/apache-tomcat-9.0.95/bin
```

Look for `startup.sh`

```shell
sudo ./startup.sh
```

Access http://localhost:8080/should_remove_1/ and see the result