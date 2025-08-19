# En este archivo está el complemento de implementación de Spring Security en el proyecto.

## 1. Documentación de Spring:
https://spring.io/projects/spring-security

## 2. Función de Spring Security: (resumen)

### Security: Spring Boot permite:

- Proteger las rutas de la API.

- Gestión de usuarios y roles.

## 3. ¿Qué es JWT (JSON Web Token)? 

Es un token de seguridad compacto y autoconclusivo que se utiliza para transmitir informacion de forma segura entre el cliente y el servidor.

## 4. Entrar a la documentación de Maven Repository:
https://mvnrepository.com/

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/53bbe5ce-bdaa-498f-a3fb-670507ae2841" />

## 5. En el proyecto que se tiene en el IDE, se debe navegar hacia el archivo "pom.xml" y agregar las dependencias:
### 5.1. Agregar la nueva dependencia de Spring Security:
````
<!-- Dependencias de Spring Security y JWT -->
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-security</artifactId>
</dependency>
````
### 5.2. Agregar la siguiente dependencia de "io.jsonwebtoken":
- Entrar a la página de Maven Repository, y buscar esa dependencia:
````
io.jsonwebtoken
````
- Elegir la versión **0.12.5**

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/f5de4cd8-9c6d-4038-abcf-00bba13bc5ca" />

- Copiar la dependencia:

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/f049cbd3-0216-4336-9fa3-5e170eca22d6" />

````
<!-- https://mvnrepository.com/artifact/io.jsonwebtoken/jjwt-api -->
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-api</artifactId>
    <version>0.12.5</version>
</dependency>
````
- Código completo de las dependencias:

````
<!-- Dependencias de Spring Security y JWT -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>
<!-- https://mvnrepository.com/artifact/io.jsonwebtoken/jjwt-api -->
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-api</artifactId>
    <version>0.12.5</version>
</dependency>
<!-- https://mvnrepository.com/artifact/io.jsonwebtoken/jjwt-impl -->
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-impl</artifactId>
    <version>0.12.5</version>
    <scope>runtime</scope>
</dependency>
<!-- https://mvnrepository.com/artifact/io.jsonwebtoken/jjwt-jackson -->
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-jackson</artifactId>
    <version>0.12.5</version>
    <scope>runtime</scope>
</dependency>
````

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/f9575217-86ef-424a-831d-857fc1b538f5" />
