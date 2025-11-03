# 00122224_practica8_secci-n1

Rene Antonio Vasquez Torres - 00122224.

-¿Cuál es la diferencia entre autenticación y autorizacion?
R//La autenticación y la autorización son procesos de seguridad secuenciales pero distintos: la autenticación es el proceso inicial que se centra en verificar la identidad del usuario o entidad, respondiendo a la pregunta "¿Quién eres?", lo cual se logra generalmente mediante credenciales como un nombre de usuario y una contraseña. Una vez que la identidad ha sido verificada satisfactoriamente (autenticación), entra en juego la autorización, que es el proceso que determina a qué recursos o acciones tiene permiso para acceder ese usuario ya identificado, respondiendo a la pregunta "¿Qué se te permite hacer?". Por ejemplo, una vez autenticado, la autorización puede permitir que un usuario vea documentos, pero no que los edite o elimine, basándose en sus roles y permisos asignados dentro del sistema.

-¿Cuál es la función del token JWT en la guía?
R//La función principal de un JSON Web Token (JWT) en un flujo de seguridad es actuar como una prueba de identidad y autorización que el servidor genera y entrega al cliente tras una autenticación exitosa. El JWT es una cadena compacta y autocontenida que incluye información sobre el usuario (conocida como claims), como su ID, roles y permisos, y está firmada digitalmente con una clave secreta para garantizar su autenticidad e integridad. De esta forma, en cada solicitud posterior, el cliente simplemente envía este token y el servidor puede verificar su firma y extraer la información de autorización necesaria sin tener que consultar repetidamente la base de datos, lo que lo hace muy eficiente para la comunicación sin estado (stateless) entre el cliente y el servidor.
