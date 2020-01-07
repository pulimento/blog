+++
title = "Ideas con RFID para organizar la ropa"
date = "2020-01-07T10:00:00+02:00"
tags = ["diy","rfid","esp32","arduino"]
draft = false
+++

Estas notas vienen de la idea de llevar el control de mi propia ropa, es decir, encontrar etiquetas pasivas lo suficientemente baratas y pequeñas para ponerlas sobre las existentes de toda mi ropa, y poder leerlas (un rango mayor a 25-30cm sería aceptable) para ver el estado de la ropa (en el bombo de la colada, en el armario, en el tendedero, etc…)

La tecnología de tiendas cashier-less (e.j. Decathlon) puede ser similar a lo que busco. Yendo más allá, lo que me he encontrado son lectores que incluso son capaz de leer varias etiquetas a la vez, y permiten mantener una trazabilidad y un posicionamiento dentro de un almacén.

No estoy buscando una solución NFC, ya que esto es más incómodo (para mi propósito, podría escanear con una cámara todas las etiquetas, o escanearlas manualmente con etiquetas RFID, pero no es mi intención. Quiero que el proceso se realice de forma automática.

Veo que el estándar que tengo que usar es el ISO 18000-6c (El EPC Gen 2 Class 1 UHF). En Europa usa (aprox)  868MHz, y en América los 960. El estándar acepta esta dualidad de frecuencias.

También pensé que las etiquetas tienen que resistir los lavados de la ropa, por lo que hay que valorar con cuidado las que están basadas en papel o cartón.

Precios que he encontrado: Aprox 8€ por 50 etiquetas - https://es.aliexpress.com/item/32772873727.html

Lectores: A partir de 45 eur (este es USB, por ejemplo, igual para unirlo a RPI/Arduino/ESP32 sería mejor RS485)
https://es.aliexpress.com/item/32801951489.html
