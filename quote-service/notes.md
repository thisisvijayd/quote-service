### java props
JAVA_HOME C:\Users\vijay\dev\graalVM\graalvm-ce-java11-20.1.0
GRAALVM_HOME C:\Users\vijay\dev\graalVM\graalvm-ce-java11-20.1.0

### graalVM
setx /M PATH "C:\Users\vijay\dev\graalVM\graalvm-ce-java8-20.1.0\bin;%PATH%"
setx /M PATH "C:\Progra~1\Java\graalvm-ce-java8-20.1.0\bin;%PATH%"
export GRAALVM_HOME="C:\Users\vijay\dev\graalVM\graalvm-ce-java8-20.1.0"
####native-image
gu install native-image

###build commands
mvnw package -Pnative
