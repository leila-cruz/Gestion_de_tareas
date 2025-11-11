# 📝 Proyecto: Tareas - Gestión de Tareas

## 📝 Descripción del proyecto
Aplicación back-end para gestionar tareas (CRUD básico, lógica de negocio y ejemplo de ejecución vía consola). Incluye ejemplos de uso de servicios, perfiles de Spring y un `CommandLineRunner` que demuestra el flujo de la aplicación en la consola.

## ⚙️ Tecnologías utilizadas
- Java 17+
- Spring Boot
- Maven (también puede ejecutarse con Gradle si el proyecto incluye wrapper)

## 🚀 Instrucciones para clonar y ejecutar el proyecto (Windows)
1. Clonar el repositorio:
git clone <URL_DEL_REPOSITORIO> cd <NOMBRE_DEL_REPOSITORIO>
2. Ejecutar con Gradle (si existe `gradlew.bat`):
.\gradlew.bat bootRun
3. Ejecutar con Maven:
mvn spring-boot:run
4. Generar JAR y ejecutar:
   - Gradle:
     ```
     .\gradlew.bat build
     java -jar build\libs\<nombre-del-jar>.jar
     ```
   - Maven:
     ```
     mvn package
     java -jar target\<nombre-del-jar>.jar
     ```

## 🔧 Cómo cambiar entre *profiles* (dev / prod)
- Usando argumentos al iniciar:
  - Gradle (Windows):
    ```
    .\gradlew.bat bootRun --args="--spring.profiles.active=dev"
    ```
  - Maven:
    ```
    mvn spring-boot:run -Dspring-boot.run.arguments="--spring.profiles.active=prod"
    ```
- Usando variable de entorno (Windows CMD):
set SPRING_PROFILES_ACTIVE=dev mvn spring-boot:run
- En IntelliJ IDEA (Run/Debug Configuration):
  - Agregar como *VM options*: `-Dspring.profiles.active=dev`
  - O en *Program arguments*: `--spring.profiles.active=prod`

## 📸 Capturas de pantalla de la consola
Incluye dos capturas de ejemplo en el directorio `screenshots`:
- salida de la consola con el profile `dev`.
<img width="1728" height="795" alt="Captura de pantalla 2025-11-10 210549" src="https://github.com/user-attachments/assets/9723e09d-d56b-4644-8280-2b4e81e1d41c" />
<img width="1643" height="789" alt="Captura de pantalla 2025-11-10 210628" src="https://github.com/user-attachments/assets/8184c2dc-9500-4223-bb2b-9f615017d699" />
<img width="1731" height="792" alt="Captura de pantalla 2025-11-10 210611" src="https://github.com/user-attachments/assets/7af45c4c-14de-4946-9444-70d0d72ec929" />



- salida de la consola con el profile `prod`.
<img width="1733" height="742" alt="Captura de pantalla 2025-11-10 210905" src="https://github.com/user-attachments/assets/5e99fa77-b9fd-4c96-94c8-63556de7d33a" />

<img width="1695" height="617" alt="image" src="https://github.com/user-attachments/assets/53c4b54b-9808-4f96-b02f-2c39e0ca9e6c" />

## 💭 Conclusiones personales sobre lo aprendido
Durante el desarrollo se afianzaron conceptos clave de Spring Boot: 
inyección de dependencias, separación entre servicios y modelo, uso de `CommandLineRunner` para tareas de arranque y la gestión de perfiles para entornos distintos. También se practicó el empaquetado y ejecución tanto con Maven como con Gradle, así como la inspección de la salida por consola para verificar el comportamiento de la aplicación.

## 👤 Nombre y legajo
- Nombre: Cruz  Leila
- Legajo: 50860


