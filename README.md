
# Setup inicial:

```
git clone https://github.com/moqui/moqui-framework.git dobleimpacto
cd dobleimpacto
git clone https://github.com/moqui/moqui-runtime.git runtime
cd runtime/component
git clone https://github.com/moqui/mantle-udm.git
git clone https://github.com/moqui/mantle-usl.git
git clone https://github.com/moqui/SimpleScreens.git
git clone https://github.com/moqui/moqui-elasticsearch.git
git clone https://github.com/dobleimpacto/moqui-crowdfunding.git
# si se tiene permiso de escritura, en lugar de la línea anterior usar acceso con ssh:
# git clone git@github.com:dobleimpacto/moqui-crowdfunding.git
cd ../..
./gradlew build
./gradlew run
```

# Acceso una vez ejecutando:

http://localhost:8080/


# Uso de IDE (actualmente sólo hay instrucciones para Intellij IDEA):

Ver instrucciones en [Moqui.org](https://moqui.org/m/docs/framework/IDE+Setup/IntelliJ+IDEA+Setup)
