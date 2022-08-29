# Requerimientos técnicos para hacer un curso de Classe

## ¿Qué ordenador necesito?

Para hacer nuestros cursos necesitas cualquier ordenador que tenga una buena potencia para desarrollar de forma fluida. Te recomendamos:

- Mínimo de 4Gb de RAM pero al ser posible 8Gb.
- Procesador i5 o similar.
- Velocidad superior a 1GHz.
- Disco duro de al menos 128Gb y si es SSD mucho mejor.

## ¿Qué sistema operativo necesito?

Puedes utilizar MacOS, Windows 10 (o superior) o Linux.

### MacOS y Linux

Si utilizas MacOS o Linux no tienes que hacer nada más.

### Windows 10

Si utilizas Windows 10 es necesario que **instales ls terminal WSL** apta para el desarrollo.
Para ello:

- Activa la opción **Subsistema de Windows para Linux**:
  - Entra en el menú inicio y busca **Activar o desactivar las características de Windows**.
  - Activa **Subsistema de Windows para Linux** y reinicia.
- Instala **Ubuntu** dentro de tu Windows:
  - Desde el menú de inicio abre **Microsoft Store**.
  - Busca **Ubuntu**.
  - Instala **Ubuntu 22.04.1 LTS**.
  - En tu menú inicio se instalará el programa **Ubuntu**, ábrelo (puede que tarde un poco).
  - Te pedirá que añadas un nuevo usuario y una contraseña: _Enter new UNIX username, New password y Retype new password_.
    Esta contraseña maestra de la terminal. La utilizarás para instalar programas así que no la pierdas.
- Ahora ya tienes instalada la misma terminal que se usa en MacOS y Linux para desarrollar. Cada vez que necesites usarla ábrela desde el menú inicio.

#### Terminal WLS de Windows en VS Code

Aunque puedes usar la terminal abriéndola desde el menú inicio también puedes configurarla para que esté integrada dentro de VS Code. Para ello:

- Abre las settings de VS Code.
- Busca **Terminal > External: Windows exec** escribiéndolo en la caja de búsqueda.
- Añade el texto **C:\Windows\System32\wsl.exe**.
- Abre una nueva terminal.
- En la parte superior de la terminal abierta hay un desplegable, ábrelo y pulsa en **Select default profile**.
- Selecciona la opción **Ubuntu (WSL)**.

> Si tienes cualquier problema para seguir estos pásos no dudes en preguntar en el canal de Slack.

