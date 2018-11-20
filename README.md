
# Setup inicial:

```
git clone https://github.com/moqui/moqui-framework.git dobleimpacto
cd dobleimpacto
./gradlew getGit -Pcomponent=SimpleScreens
./gradlew getGit -Pcomponent=moqui-elasticsearch
cd runtime/component
git clone https://github.com/dobleimpacto/moqui-crowdfunding.git
git clone https://github.com/moitcl/moqui-chile # Opcional, agrega localización para Español/Chile
cd ../..
./gradlew run
```

## Descripción:

Con este setup se tiene acceso a la funcionalidad básica de Moqui.

Con la tarea "run", se descargan dependencias, se compila y se puebla una base de datos H2 que está configurada por defecto, incluyendo datos de demostración.

Si se quiere conocer un poco más del funcionamiento, modelo de datos, etc, se puede instalar además algún componente que incorpora aplicaciones adicionales (no necesarias para usar moqui-crowdfunding).

```
./gradlew getGit -Pcomponent=HiveMind
./gradlew getGit -Pcomponent=PopCommerce
```

Si ya se habían cargado los datos iniciales, o si se quiere volver al estado inicial, usar:

```
./gradlew cleanDb load run
```

# Acceso una vez ejecutando (gradlew run):

http://localhost:8080/


# Uso de IDE (actualmente sólo hay instrucciones para Intellij IDEA):

Ver instrucciones en [Moqui.org](https://moqui.org/m/docs/framework/IDE+Setup/IntelliJ+IDEA+Setup)
