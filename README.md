# RMM-2022-GETT
Proyecto horas B de configuración de centralita ASTERISK

# Centralita telefónica de VoIP basada en Asterisk
Este proyecto consiste en la instalación y configuración de una centralita telefónica de VoIP basada en Asterisk. La centralita actuará también como proxy SIP para los terminales, asociados siempre a ella a través de canales SIP.

## Autores
Autor 1: Fernando de Peroy Rodríguez - [@fernandodpr](https://github.com/fernandodpr/)

Autor 2: Santiago Esparis Matanza - [@Santiago-Esparis](https://github.com/Santiago-Esparis)
## Objetivo
El objetivo de este proyecto es configurar una centralita telefónica de VoIP basada en Asterisk con las funcionalidades básicas y avanzadas requeridas para que la práctica sea evaluada favorablemente.

## Funcionalidades básicas
La centralita contará con 10 extensiones de voz, de la 100 a la 109, con contraseñas respectivas:
rmm23.100, rmm23.101, …, rmm23.109
Cada una de estas extensiones tendrá asociado un buzón de voz (con contraseñas 0100, …, 0109).
Mientras no se establezca la llamada, la centralita amenizará la espera del usuario llamante con una agradable música de fondo. Si transcurridos 8 segundos la llamada aún no ha sido establecida, entonces será redirigida al buzón de voz de la extensión correspondiente.
La centralita contará con un menú IVR ligado a la extensión 900 que dará acceso a los siguientes servicios:

1. Acceso al buzón de voz del usuario.
2. Servicio “no molestar”: cuando un usuario active este servicio, dejará de recibir llamadas y todas sus llamadas entrantes serán redirigidas directamente a su buzón de voz. Desde esta opción del menú, el usuario podrá habilitar/deshabilitar este servicio en cualquier momento.
3. Servicio IP: la centralita informará al usuario de la dirección IP y el número de puerto desde los que se ha conectado.
La centralita reproducirá un mensaje de error al usuario que intente realizar una llamada a un número que no se corresponda con ninguna de las extensiones internas.
## Funcionalidades avanzadas
En este apartado se proponen varios servicios que la centralita podría soportar opcionalmente. Para poder alcanzar la máxima calificación, la centralita deberá proporcionar alguno de los siguientes servicios (en la opción 4 del menú IVR):

- Servicio "currency converter": el usuario puede obtener el equivalente en dólares de una determinada cantidad de euros (y viceversa). La centralita utiliza el tipo de cambio oficial en tiempo real y proporciona el resultado con una precisión de hasta dos decimales.
  - El valor deseado se debe introducir empleando # como separador decimal.
  - Previa solicitud del valor al usuario la centralita lee en alto el valor actual de cambio.



