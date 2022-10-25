+++
title = "Comunicación cliente-servidor"
tags = ["comunicacion"]
banner = "../img/cliente_servidor.png"
authors = ["Andrés"]
+++

## Con mis propias palabras

La **comunicación entre cliente y servidor** es aquella en la que se solicita una **petición** por parte del cliente, ésta se **transmite** por la red a un servidor (mediante una URL) el cual responde si dispone o no, si tiene autorizaición o no del **recurso** solicitado y se lo devuelve a través de la red al cliente. 



[![](https://mermaid.ink/img/pako:eNpNkE1ugzAUhK_y5DVcgEUlA1ZKlQLCTrooLFxsCmr4kW0iVXFO0SP1YnVwqtbywu955htpLqidhUQReld86YGl9QTu4NeORx0Pu0FJyPGR7HBaVA2E4YN9ZKyEHWFQEpYl2fdXbiG-67VUZ6mAkuqYOQO8kLjxxPjPWxFaHghl2AL-9wn2UO1t8ktaBuFIuNxnCU6yIt9YN0ZvxlPYah088TPXrRoWY2PPSbYQwc2sLaR3khv5G9cSYkwJpO5iVtDGR3pt4u0oQKNUIx-EK-Ry29XI9HKUNYrcU3D1UaN6ujodX81MP6cWRUatMkDr4kgyHbjrcUQu9qTdVorBzOrZN7wVff0Bg2xzgA?type=png)](https://mermaid.live/edit#pako:eNpNkE1ugzAUhK_y5DVcgEUlA1ZKlQLCTrooLFxsCmr4kW0iVXFO0SP1YnVwqtbywu955htpLqidhUQReld86YGl9QTu4NeORx0Pu0FJyPGR7HBaVA2E4YN9ZKyEHWFQEpYl2fdXbiG-67VUZ6mAkuqYOQO8kLjxxPjPWxFaHghl2AL-9wn2UO1t8ktaBuFIuNxnCU6yIt9YN0ZvxlPYah088TPXrRoWY2PPSbYQwc2sLaR3khv5G9cSYkwJpO5iVtDGR3pt4u0oQKNUIx-EK-Ry29XI9HKUNYrcU3D1UaN6ujodX81MP6cWRUatMkDr4kgyHbjrcUQu9qTdVorBzOrZN7wVff0Bg2xzgA)


graph TD
    A[fa:fa-fire NAVEGADOR] -->|HTTP GET PETICIÓN| B[fa:fa-server SERVIDOR WEB]
    B -->|HTTP RESPUESTA| A
    B --> |URL|C[fa:fa-spider APLICACION WEB]-->|html-css,Javascript|B
    C -->|datos| D[fa:fa-database BASE DE DATOS] --> |datos|C