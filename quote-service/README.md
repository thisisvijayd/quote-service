# quote-service project

This project uses Quarkus, the Supersonic Subatomic Java Framework.

reference https://quarkus.io/ .

## Running the application in dev mode 
./mvnw quarkus:dev

###
build native mvnw package -Pnative

## Packaging and running the application

The application can be packaged using `./mvnw package`.
It produces the `quote-service-1.0.0-SNAPSHOT-runner.jar` file in the `/target` directory.
Be aware that it’s not an _über-jar_ as the dependencies are copied into the `target/lib` directory.

The application is now runnable using `java -jar target/quote-service-1.0.0-SNAPSHOT-runner.jar`.

## Creating a native executable

You can create a native executable using: `./mvnw package -Pnative`.

Or, if you don't have GraalVM installed, you can run the native executable build in a container using: `./mvnw package -Pnative -Dquarkus.native.container-build=true`.

You can then execute your native executable with: `./target/quote-service-1.0.0-SNAPSHOT-runner`

If you want to learn more about building native executables, please consult https://quarkus.io/guides/building-native-image.



###Detailed steps

#### Create quarkus code using initialiser
#### Install graalVM
#### gu install native-image
#### native image requires visual studio code x64 
x64 Native Tools Command Prompt for VS 2019
Otherwise you will see this issue 
* Native-image building on Windows currently only supports target architecture: AMD64 (x86 unsupported)
https://github.com/oracle/graal/issues/2116
