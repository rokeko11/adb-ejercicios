
## Escalabilidad Vertical vs. Escalabilidad Horizontal

### Escalabilidad Vertical
- **Definición:** La escalabilidad vertical, también conocida como "scale-up," se refiere al proceso de agregar recursos a una sola máquina para aumentar su capacidad. Esto puede incluir la adición de más CPU, memoria RAM, almacenamiento o una mejor tarjeta gráfica.
  
- **Ventajas:**
  - Más sencillo de implementar, ya que implica menos cambios en la arquitectura de la aplicación.
  - Mantiene la lógica de la aplicación en una sola instancia.
  
- **Inconvenientes:**
  - Existe un límite en cuanto a cuántos recursos se pueden agregar a una única máquina.
  - Puede ser costoso, ya que los componentes de hardware de alta gama suelen ser más caros.

### Escalabilidad Horizontal
- **Definición:** La escalabilidad horizontal, también conocida como "scale-out," implica agregar más máquinas o nodos a un sistema para distribuir la carga y aumentar la capacidad total. Esto permite que el sistema maneje más usuarios o datos mediante la adición de más servidores.
  
- **Ventajas:**
  - No hay un límite teórico en la cantidad de máquinas que se pueden agregar.
  - Generalmente, es más rentable, ya que se pueden usar servidores más baratos y menos potentes.
  - Mejora la tolerancia a fallos, ya que si un servidor falla, otros pueden seguir funcionando.
  
- **Inconvenientes:**
  - Puede ser más complejo de implementar y gestionar, ya que requiere un diseño de sistema que distribuya la carga de manera eficiente.
  - Necesita una infraestructura de red robusta para conectar múltiples servidores.

## SGBD que Permiten Mejor Escalado Horizontal

Algunos sistemas de gestión de bases de datos (SGBD) que permiten un mejor escalado horizontal incluyen:

1. **MongoDB:**
   - Es una base de datos NoSQL orientada a documentos que permite la fragmentación de datos (sharding), lo que facilita la distribución de datos a través de múltiples servidores.

2. **Cassandra:**
   - Diseñada para manejar grandes volúmenes de datos distribuidos en múltiples nodos, Cassandra permite la replicación y la fragmentación, lo que la hace altamente escalable.

3. **Couchbase:**
   - Esta base de datos NoSQL combina las características de una base de datos de documentos y de clave-valor, y ofrece soporte para la escalabilidad horizontal a través de la distribución de datos en varios nodos.

4. **Amazon DynamoDB:**
   - Un servicio de base de datos NoSQL completamente gestionado que permite la escalabilidad horizontal sin que el usuario tenga que preocuparse por la infraestructura subyacente.

5. **Google Cloud Spanner:**
   - Ofrece una base de datos SQL completamente gestionada que combina la consistencia de las bases de datos relacionales con la escalabilidad horizontal de las bases de datos NoSQL.

