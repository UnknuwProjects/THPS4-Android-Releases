# THPS4 — Port não oficial para Android

[English](README.md) · [Bahasa Indonesia](README.id.md) · [Español](README.es.md) · **Português**

Um port não oficial de **Tony Hawk's Pro Skater 4** (Xbox) para Android,
recompilado de forma estática para rodar nativamente em celulares ARM64.

> **Este repositório é apenas o canal público de lançamentos.** O
> desenvolvimento acontece em um repositório privado; o que fica aqui é este
> README e os lançamentos estáveis — sem código-fonte e **sem dados do jogo**.

## O jogo não está incluído

Este port não contém nenhum arquivo do jogo. Para jogar, você fornece **os
seus próprios dados originais do jogo ou o seu arquivo ISO** e os coloca na
pasta `THPS4` do armazenamento compartilhado do celular:

```
/storage/emulated/0/THPS4/
```

O launcher verifica a pasta para você e mostra o que encontrou.

## A sua cópia é oficial?

Esta página é o único lugar onde este port é lançado. Todas as builds
oficiais são assinadas com o mesmo certificado, impressão digital SHA-256:

```
12474f52e9b6a461bceb2af6882a0543d8dc6e49fc8fcb06ac25de83489885bb
```

A partir da 1.0.4, o próprio jogo confere isso ao iniciar e para se uma
cópia tiver sido reassinhada. Cópias de outros sites podem trazer código
extra inserido nelas — não são nossas, e o que uma cópia dessas fizer não
faz parte deste projeto.

## Recursos

- O jogo completo: Carreira, Free Skate, Create-A-Skater, Park Editor, 2 jogadores em tela dividida
- Inglês / **tradução completa para indonésio**, alternável no launcher e dentro do jogo
- Ajustes do Port dentro do menu Options do próprio jogo (gráficos, idioma, créditos)
- Opções gráficas: escala de renderização, limite de FPS, VSync, antialiasing, filtros de tela, ultrawide, bloom, névoa
- Medidor de desempenho na tela: FPS, nome da GPU, carga e temperatura da GPU, CPU, RAM, bateria
- Suporte a mods: pacotes de mods (texturas, shapes, sons, modelos, fases), skaters personalizados, pacotes de texturas
- Sua própria música: o sistema de trilha sonora personalizada do jogo (WMA) e um player My Music (MP3/OGG/FLAC/…)
- Multiplayer System Link por LAN, controles por gamepad / teclado / mouse / toque
- Um launcher antes do jogo: status da pasta do jogo, gerenciador de mods, gerenciador de músicas, verificação de atualizações

## Requisitos

- Android 10 ou superior (API 29+), aparelho ARM64
- A sua própria cópia do jogo (veja acima)

## Instalação

1. Baixe o APK mais recente em [Releases](../../releases).
2. Instale (todas as builds são assinadas com a mesma chave, então as atualizações instalam por cima da versão anterior).
3. Coloque os dados do jogo ou o ISO na pasta `THPS4`.
4. Abra o **THPS4** e toque em **Launch Game**.

O launcher também verifica este repositório em busca de atualizações e pode
baixar a próxima versão para você.

## Jogar online

**Na mesma Wi-Fi**: o System Link (até 8 jogadores) e o 2P Online
(2 jogadores) funcionam na sua rede local sem configurar nada: um celular é
o host e o outro entra com o código do host, da página Multiplayer do painel.

**Em redes diferentes**: celulares atrás do NAT da operadora não se alcançam
diretamente. Há dois caminhos para resolver isso:

- **App de VPN (funciona hoje):** instale o Tailscale (grátis para uso
  pessoal) nos dois celulares e entre com a mesma conta nos dois. Cada
  celular recebe um endereço `100.x.x.x` — use o do host como destino no
  painel, igual a um endereço de LAN. O System Link pela VPN comporta até
  8 jogadores, igual à LAN.
- **Salas online (chegam na 1.0.4):** o painel ganha o Multiplayer Port —
  salas públicas em um servidor da comunidade. Crie uma sala ou entre em uma
  da lista; sem app extra, sem códigos para trocar. Uma sala comporta
  2 jogadores (é o modo local de 2 jogadores do jogo, jogado pela internet),
  e muitas salas podem rodar ao mesmo tempo. A mesma lista também traz as
  salas link: sessões de System Link pela internet para até 8 jogadores,
  marcadas como LINK na lista.

Seja qual for o caminho, os dois celulares precisam rodar a **mesma versão
com os mesmos mods** e escolher a **mesma fase** — o 2P Online troca apenas
as entradas do controle e cada celular roda a sua própria cópia do jogo,
então dados diferentes não conseguem ficar em sincronia. As salas da lista
são marcadas quando o conjunto de mods delas difere do seu, e o painel pode
baixar os pacotes do host para você — depois de reiniciar uma vez, o seu
conjunto fica igual ao da sala.

## Versões

Os lançamentos daqui usam versionamento semântico estável — `MAJOR.MINOR.PATCH`
(primeiro lançamento público: **1.0.0**). As notas de cada lançamento listam
o que mudou. As builds de desenvolvimento (a linha `beta`) são testadas em
particular e não são publicadas aqui; uma build é publicada quando é
considerada estável.

## Relatos de bugs

Encontrou um bug? Relate na
[página de Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
com o modelo do seu celular, a sua versão do Android e o que aconteceu. Se
puder, anexe o arquivo `thps4.log` da pasta `THPS4/logs` do seu
armazenamento — esse log torna a maioria dos bugs corrigível.

## Créditos e apoio

Port de **UNKNUW** — [github.com/UnknuwProjects](https://github.com/UnknuwProjects)

Apoie o projeto:
[Sociabuzz](https://sociabuzz.com/unknuw/tribe) ·
[Saweria](https://saweria.co/Unknuw)

*Projeto de fã não oficial. Sem afiliação com a Activision ou a Neversoft.
Tony Hawk's Pro Skater 4 é uma marca de seus respectivos proprietários.*
