---
layout: post
title:  "Python - Verificando Espaço em Disco do Servidor"
date:   2020-01-12 23:30:00 -0300
categories: python linux ubuntu rocketchat azure
---

Olá,

Estou gerenciando um servidor Ubuntu dentro do [Azure][Azure] e tive problemas de espaço em disco devido ao log do Apache em Docker. No meu ambiente, o espaço em disco do servidor estava, devido um erro na aplicação, sendo consumido 100%, travando a aplicação.

Nas configurações da VM, não tenho avisos por espaço em disco, ou seja, estava com um problema para resolver.

Como utilizamos o [Rocket.chat][Rocket.chat] para comunicação dentro da empresa, resolvi então criar um script para verificar o espaço em disco do servidor e se o consumo estiver acima ou igual a 80% da capacidade, enviar uma mensagem em um canal do Rocket.chat específico. Este script está rodando em uma cron no servidor 1x ao dia e já resolveu o meu problema.

Segue o link do Script para ser utilizado: [Aviso Rock][Aviso Rock].

Veja que utilizei a biblioteca [psutil][psutil] da linguagem [Python][Python]. Esta biblioteca é fantástica, acho que seria legal você estudar ela.

Obrigado!

[Azure]: https://azure.microsoft.com/pt-br/
[Rocket.chat]: https://rocket.chat/
[Aviso Rock]: https://github.com/gmantovani2005/python-infra/blob/master/disco/sendrock.py
[psutil]: https://psutil.readthedocs.io/en/latest/
[Python]: https://www.python.org/
