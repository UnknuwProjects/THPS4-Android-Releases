# THPS4 — Port no oficial para Android

[English](README.md) · [Bahasa Indonesia](README.id.md) · **Español** · [Português](README.pt.md)

Un port no oficial de **Tony Hawk's Pro Skater 4** (Xbox) para Android,
recompilado de forma estática para correr de forma nativa en teléfonos ARM64.

> **Este repositorio es solo el canal público de versiones.** El desarrollo se
> hace en un repositorio privado; lo que vive aquí es este README y las
> versiones estables: sin código fuente y **sin datos del juego**.

## El juego no está incluido

Este port no contiene ningún archivo del juego. Para jugar, aportas **tus
propios datos originales del juego o tu archivo ISO** y los colocas en la
carpeta `THPS4` del almacenamiento compartido de tu teléfono:

```
/storage/emulated/0/THPS4/
```

El launcher revisa la carpeta por ti y te muestra lo que encontró.

## ¿Tu copia es oficial?

Esta página es el único lugar donde se publica este port. Todas las builds
oficiales se firman con el mismo certificado, huella SHA-256:

```
12474f52e9b6a461bceb2af6882a0543d8dc6e49fc8fcb06ac25de83489885bb
```

Desde la 1.0.4, el propio juego lo comprueba al arrancar y se detiene si una
copia fue refirmada. Las copias de otros sitios pueden llevar código extra
añadido en su interior: no son nuestras, y lo que haga una copia así no forma
parte de este proyecto.

## Características

- El juego completo: Carrera, Free Skate, Create-A-Skater, Park Editor, 2 jugadores a pantalla partida
- Inglés / **traducción completa al indonesio**, cambiable en el launcher y dentro del juego
- Ajustes del Port dentro del menú Options del propio juego (gráficos, idioma, créditos)
- Opciones gráficas: escala de renderizado, límite de FPS, VSync, antialiasing, filtros de pantalla, ultrawide, bloom, niebla
- Medidor de rendimiento en pantalla: FPS, nombre de la GPU, carga y temperatura de la GPU, CPU, RAM, batería
- Soporte de mods: paquetes de mods (texturas, tablas, sonidos, modelos, niveles), skaters personalizados, paquetes de texturas
- Tu propia música: el sistema de banda sonora personalizada del juego (WMA) y un reproductor My Music (MP3/OGG/FLAC/…)
- Multijugador System Link por LAN, controles de mando / teclado / ratón / táctiles
- Un launcher previo al juego: estado de la carpeta del juego, gestor de mods, gestor de música, búsqueda de actualizaciones

## Requisitos

- Android 10 o superior (API 29+), dispositivo ARM64
- Tu propia copia del juego (ver arriba)

## Instalación

1. Descarga el APK más reciente desde [Releases](../../releases).
2. Instálalo (todas las builds se firman con la misma clave, así que las actualizaciones se instalan sobre la versión anterior).
3. Coloca tus datos del juego o tu ISO en la carpeta `THPS4`.
4. Abre **THPS4** y pulsa **Launch Game**.

El launcher también consulta este repositorio en busca de actualizaciones y
puede descargar la siguiente versión por ti.

## Jugar en línea

**La misma Wi-Fi**: System Link (hasta 8 jugadores) y 2P Online (2 jugadores)
funcionan en tu red local sin configurar nada: un teléfono hace de host y el
otro se une con el código de host de la página Multiplayer del panel.

**Redes distintas**: los teléfonos tras el NAT de la operadora no pueden
alcanzarse directamente. Hay dos formas de resolverlo:

- **App de VPN (funciona hoy):** instala Tailscale (gratis para uso personal)
  en ambos teléfonos e inicia sesión con la misma cuenta en los dos. Cada
  teléfono recibe una dirección `100.x.x.x`: usa la del host como destino en
  el panel, igual que una dirección LAN. System Link por la VPN admite hasta
  8 jugadores, igual que en una LAN.
- **Salas en línea (llegan en la 1.0.4):** el panel gana Multiplayer Port:
  salas públicas en un servidor comunitario. Crea una sala o únete a una de
  la lista; sin apps extra y sin códigos que intercambiar. Una sala admite
  2 jugadores (es el modo local de 2 jugadores del juego, jugado por
  internet), y muchas salas pueden funcionar al mismo tiempo. La misma lista
  también lleva salas link: sesiones de System Link por internet para hasta
  8 jugadores, marcadas como LINK en la lista.

Uses la ruta que uses, ambos teléfonos deben correr la **misma versión con
los mismos mods** y elegir el **mismo nivel**: 2P Online solo intercambia
las entradas del mando y cada teléfono ejecuta su propia copia del juego,
así que unos datos distintos no pueden mantenerse en sincronía. Las salas
de la lista se marcan cuando su conjunto de mods difiere del tuyo, y el
panel puede descargar los paquetes del host por ti: tras un reinicio, tu
conjunto coincide con el de la sala.

## Versiones

Las versiones de aquí usan versionado semántico estable: `MAJOR.MINOR.PATCH`
(primera versión pública: **1.0.0**). Las notas de cada versión enumeran los
cambios. Las builds de desarrollo (la rama `beta`) se prueban en privado y
no se publican aquí; una build se publica cuando se considera estable.

## Informes de errores

¿Encontraste un error? Infórmalo en la
[página de Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
con el modelo de tu teléfono, tu versión de Android y lo que pasó. Si
puedes, adjunta el archivo `thps4.log` de la carpeta `THPS4/logs` de tu
almacenamiento: ese registro hace que la mayoría de los errores se puedan
corregir.

## Créditos y apoyo

Port de **UNKNUW** — [github.com/UnknuwProjects](https://github.com/UnknuwProjects)

Apoya el proyecto:
[Sociabuzz](https://sociabuzz.com/unknuw/tribe) ·
[Saweria](https://saweria.co/Unknuw)

*Proyecto de fans no oficial. Sin afiliación con Activision ni Neversoft.
Tony Hawk's Pro Skater 4 es una marca de sus respectivos propietarios.*
