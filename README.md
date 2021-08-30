# Telegram_bot_Api_Notification
Avisos Telegram_bot via API

La intención de este script es poder automatizar los avisos desde un equipo que pueda leer este script y asi dar aviso via la API de telegram.

El uso de este es de la siguiente forma:

telegram.notify TOKEN ID "Mensaje a enviar"

#######################################################################
#
#             CREAR UN BOT EN TELEGRAM
#
#######################################################################

Como crear un bot en Telegram


Primer paso para crear un Bot

Los pasos como crear un Bot con @BotFather, que es el padre de todos los Bots, creado por Telegram con el fin de facilitar la creación de estos:

Hacemos clickamos este enlace @BotFather e iniciamos el Bot.

Seleccionamos o escribimos /newbot. Nos preguntará: 
¿Que nombre quieres dar a tu bot?. Escribimos un nombre.

El Bot nos respone ahora: 
¿Que nick quieres usar para este bot?, 
recuerda que el nick debe de acabar en bot o _bot. ejem: @nick_bot, @nickbot,…


@BotFather ya nos ha creado el bot!!!. 
Ahora ya tenemos nuestro numero de Token para poder utilizar nuestro bot.



Ingresa a tu bot y dale Iniciar/Start

Cada usuario y grupo en Telegram tiene un identificador, ID.

Si queremos añadir el Bot en un Grupo o Canal, para que envíe mensajes o haga cualquier función, tendremos que averiguar el ID de ese Grupo o Canal. 

Para ello abre un navegador y escrfibe lo siguiente:

https://api.telegram.org/bot[TOKEN DEL BOT]/GetUpdates   <-- sin los corchetes y todo junto

Envia un mensaje al bot desde telegram y podras ver tu ID en el GetUpdate del navegador en un formato parecido a este:

{
  "message_id":2,
  "from":{
    "id":Numero_ID,     <--- Los IDs de los usuarios son numeros positivos y los IDs de grupos son numeros negativos
    "is_bot":false,
    "first_name":"Nombre",
    "last_name":"Usuario",
    "username":"Username",
    "language_code":"es"
    },
    
    
    Recuerda tu TOKEN y Recuerda tu ID
    
    
    En tu maquina clona el repositorio o copia el script como te acomode
    
    dale permisos de ejecucion al script con:
    
    sudo chmod +x telegram.notify
    
    y ya lo puedes ejecutar con ./telegram.notify
    
    Si lo quieres dejar como binario de sistema solo copialo al /usr/bin
    
    cp telegram.notify /usr/bin y podrás llamarlo de cualquier parte del sistema
