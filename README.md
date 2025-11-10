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
<img width="900" height="431" alt="image" src="https://github.com/user-attachments/assets/4154d336-9adc-44ff-932d-e6cc8014baa7" />
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
- `screenshots/console-dev.png` — salida de la consola con el profile `dev`.
- `screenshots/console-prod.png` — salida de la consola con el profile `prod`.

(Para generar las capturas: ejecutar con el profile deseado y usar la herramienta de recorte de Windows o `PrtSc`, luego guardar en la ruta indicada.)

## 💭 Conclusiones personales sobre lo aprendido
Durante el desarrollo se afianzaron conceptos clave de Spring Boot: 
inyección de dependencias, separación entre servicios y modelo, uso de `CommandLineRunner` para tareas de arranque y la gestión de perfiles para entornos distintos. También se practicó el empaquetado y ejecución tanto con Maven como con Gradle, así como la inspección de la salida por consola para verificar el comportamiento de la aplicación.

## 👤 Nombre y legajo
- Nombre: Cruz  Leila
- Legajo: 50860


