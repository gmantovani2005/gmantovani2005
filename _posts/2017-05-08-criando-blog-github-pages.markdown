---
layout: post
title:  "Criando Blog no GitHub Pages com Linux Mint e Jekyll"
date:   2017-05-08 09:00:00 -0000
categories: jekyll linux mint github git ruby
---

![Meu screenshot]({{ site.url }}/assets/criando-blog-github-jekyll.png)

Vou demonstrar hoje como criei meu blog utilizando o [GitHub Pages][GitHub-Pages], que é um serviço do [GitHub][GitHub] para prover páginas de internet. Estas páginas podem ser utilizadas para divulgar exemplos, demos, documentações e qualquer outro tipo de informação sobre o seu projeto. Acesse a página do GitHub Pages e siga os passos da página inicial para criar sua primeira página. Muito simples.

Eu fiz um pouco diferente do que explica a página. Segui os seguintes passos:

* Instalei o [Jekyll][Jekyll]
* Criei um blog com o Jekyll
* Criei um repositório vazio no GitHub (usuario.github.io)
* Subi meu blog para o repositório do Github

## No Linux Mint, digitei os seguintes comandos:

{% highlight Bash shell scripts %}
$ sudo apt install jekyll
$ jekyll new blog
$ cd blog
$ git add .
$ git commit -am 'Primeiro commit do blog'
$ git push
{% endhighlight %}

Pronto! Tudo rodando. Agora é só fazer as alterações na página quando necessário e fazer o commit. Isto pode ser feito de várias jeitos. Você pode dentro do GitHub criar/alterar as páginas conforme sua necessidade. Ou pode fazer localmente e subir com commit/push para o seu repositório.

Eu estou fazendo local por enquanto, pois posso testar a página antes de subir, ver como está ficando.

[GitHub]: https://github.com/
[GitHub-Pages]: https://pages.github.com/
[Jekyll]: https://jekyllrb.com/
