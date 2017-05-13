---
layout: post
title:  "Criando um Pendrive de Inicialização do XUbuntu"
date:   2017-05-13 10:00:00 -0300
categories: linux pendrive boot ubuntu xubuntu
---

Estes dias fui fazer um teste com o [XUbuntu][XUbuntu] e para isto precisava de um pendrive para a instalação.

Toda vez que precisava de um pendrive ou DVD de qualquer sistema operacional, eu sempre utilizava uma ferramenta. Desta vez fiz diferente e na minha opinião de uma forma bem mais simples.

Eu apenas baixei a ISO do XUbuntu e fiz o seguinte comando no terminal do Linux (como root):

{% highlight Bash shell scripts %}
# cat arquivo.iso > /dev/sdb
{% endhighlight %}

**Cuidado:** este comando irá apagar tudo que estiver no arquivo e irá extrair os arquivos da imagem (ISO) para o pendrive.

**Só para ficar registrado:** Adorei a interface gráfica [Xfce][Xfce]. Numa havia trabalhado nela por muito tempo. É simples. Tem tudo que preciso.

[XUbuntu]: https://xubuntu.org/
[Xfce]: https://www.xfce.org/
