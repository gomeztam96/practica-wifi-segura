# practica-wifi-segura

Introducción 

Cuando nos conectamos a una red Wi-Fi pública, como la de un café, aeropuerto o universidad, nuestro dispositivo intercambia información con diferentes servidores a través de la red. Si una página utiliza HTTP en lugar de HTTPS, parte de esa comunicación puede viajar sin cifrado. 

En esta práctica se analizó una conexión HTTP utilizando las herramientas de desarrollador del navegador. 

Sitio analizado 

El sitio utilizado para la práctica fue: 

http://sublimegrandshiningchart.neverssl.com/online/ 

El sitio utiliza HTTP, no HTTPS. 

Datos observados 

Request URL: http://sublimegrandshiningchart.neverssl.com/online/ 

Request Method: GET 

Status Code: 200 OK 

Remote Address: 2600:1f13:37c:1400:ba21:7165:5fc7:736e:80 

Puerto: 80 

Referrer Policy: strict-origin-when-cross-origin 

1. ¿Qué protocolo utiliza el sitio? 

El sitio utiliza HTTP (Hypertext Transfer Protocol). 

Esto se puede comprobar porque la dirección comienza con http:// y la conexión utiliza el puerto 80. 

A diferencia de HTTPS, HTTP no cifra mediante TLS el contenido de la comunicación entre el navegador y el servidor. Por eso, no debe utilizarse para transmitir información sensible, especialmente cuando estamos conectados a una red Wi-Fi pública. 

2. ¿Qué información puede observarse durante la solicitud? 

Durante el análisis de la solicitud HTTP se pudieron observar diferentes elementos: 

Host / servidor: sublimegrandshiningchart.neverssl.com 

URL: http://sublimegrandshiningchart.neverssl.com/online/ 

Método: GET 

Headers: información adicional enviada en la solicitud HTTP. 

Remote Address: dirección del servidor al que se realizó la conexión. 

Puerto: 80, correspondiente a HTTP. 

Status Code: 200 OK, que indica que la solicitud fue procesada correctamente. 

Estos datos permiten observar cómo se establece la comunicación entre el navegador y el servidor. 

3. ¿Qué riesgos existen al navegar mediante HTTP desde una red Wi-Fi pública? 

Utilizar HTTP en una red Wi-Fi pública presenta riesgos porque la comunicación no cuenta con el cifrado que proporciona HTTPS. 

Un atacante que consiga observar el tráfico de la red podría llegar a obtener información que viaje sin cifrar, como las páginas o recursos solicitados y determinados datos incluidos en las comunicaciones HTTP. 

Esto puede facilitar ataques de interceptación o espionaje del tráfico, especialmente si se transmiten datos sensibles mediante HTTP. 

Por este motivo, no es recomendable ingresar contraseñas, datos bancarios u otra información privada en sitios que utilizan HTTP. 

4. ¿Cómo cambiaría este escenario utilizando una VPN? 

Una VPN establece un túnel cifrado entre el dispositivo del usuario y el servidor VPN. 

De esta manera: 

Cifrado: el tráfico entre el dispositivo y la VPN viaja cifrado. 

Túnel seguro: la VPN encapsula el tráfico dentro de una conexión protegida. 

Protección del tráfico: dificulta que otros usuarios de la misma red Wi-Fi puedan observar directamente el contenido del tráfico protegido. 

Privacidad: el sitio web normalmente verá la dirección IP del servidor VPN en lugar de la dirección IP pública original del usuario. 

Una VPN mejora la protección al utilizar una Wi-Fi pública, aunque no reemplaza otras medidas de seguridad, como utilizar HTTPS, mantener los dispositivos actualizados y evitar ingresar información sensible en sitios que no utilizan conexiones seguras. 

5. Mis 3 Reglas de Oro para navegar en redes Wi-Fi públicas 

Regla 1 — Usar HTTPS 

Antes de ingresar información personal, contraseñas o datos bancarios, comprobar que el sitio utilice https://. 

️ Regla 2 — Utilizar una VPN cuando sea necesario 

En redes Wi-Fi públicas, utilizar una VPN confiable para proteger el tráfico mediante un túnel cifrado. 

 Regla 3 — Evitar operaciones sensibles en redes públicas 

Evitar realizar operaciones bancarias o ingresar información muy sensible cuando estoy conectado a una red Wi-Fi pública que no considero confiable. 

Evidencia observada 

Durante la práctica se utilizó la herramienta Network de las herramientas de desarrollador del navegador. 

La solicitud analizada mostró: 

Método GET 

Código 200 OK 

Puerto 80 

URL utilizando http:// 



 


