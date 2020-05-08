# Instruções Para os Membros

## Como criar sua pagina de membro

Se você é um novo membro, siga essas instruções:

<ol>
<li>Crie o arquivo <code>seu_nome.md</code> dentro da pastas <code>_authors</code>, por exemplo: <code>_authors/anthony.md</code></li>
<li>Dentro do aquivo insira o texto:
   
```
---
short_name: o nome que irá assinar os posts
name: seu nome
position: sua ocupação  
---
um texto sobre você
```
</li>
</ol> 

Agora você você já ira aparecer na pagina de membros do site.

## Como fazer uma postagem em seu nome

Todas as postagens devem estar em arquivos `.md` dentro da pasta `_posts`

<ol>
<li>
Crie o arquivo no formato <code>ANO-MES-DIA-ENDERECO.md</code> dentro da pasta  <code>_posts</code>,<br>por exemplo:
<code>_authors/2020-04-18-ann1.md</code></li>
<li>Dentro do aquivo insira o texto:

```
 ---
layout: post
title: "Titulo do post"
author: Seu short_name
---
corpo do texto
```
</li>
</ol>
Sua publicação estará no endereço <code>anthonyaposta.github.io/ANO/MES/DIA/ENDERECO.html</code>

Agora você ja sabe como fazer posts. 

# Rodando o site localmente

É possivel editar os site diretamente pelo github, mas essa não é a melhor forma. Durante a edição de um novo conteudo 
queremos ver o resultado e realizar mudanças antes de atualizar o site diretamente, isso pode ser feito rodando [Jekyll](https://jekyllrb.com/) (programa que gera o site) no seu computador.

## Bora lá!
 
Veja qual sistema operacioal você está utilizando e instale as depedências:

Ubuntu:

```sudo apt-get install ruby-full build-essential zlib1g-dev```

Debian:

```sudo apt-get install ruby-full build-essential```

ArchLinux:

```sudo pacman -S ruby base-devel```

Caso seu sistema não esteja listado, clique [aqui](https://jekyllrb.com/docs/installation/other-linux/).

As proximas instruções são comuns a todos os sistemas:

Para configurar o caminho de instalação:

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
Para instalar:

```gem install jekyll bundler```

blz, agora é so clonar o repositorio no seu PC e dentro do repo rodar o comando

```bundle exec jekyll serve```

clque no link em ```Server address:```  para abrir o site.

Mais ifos sobre a instalação do Jekyll em [https://jekyllrb.com/docs/installation/ubuntu/](https://jekyllrb.com/docs/installation/ubuntu/)

# FIM! 
