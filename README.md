# novosh
Muitas vezes precisamos criar alguns scripts rápidos para fazer alguns teste e ter que fazer todo um cabeçalho toda vez que precisamos criar um script se torna uma tarefa chata e repetitiva. Esse script tem como obtivo automatizar essa tarefa.
Para tanto:
- copie o arquivo novosh para: <b>~/.local/bin</b>
- dê as permissoes de execução: <b>chmod +x novosh</b> 
- adicione o diretório anterior ao seu PATH: <b>echo "export PATH=$HOME/.local/bin:$PATH" >> ~/.bashrc </b>
- recarregue suas configurações: <b>source ~/.bashrc</b>

Assim você poderá executar de qualquer lugar o comando:

<code>
  $ novosh
</code>


O script vai pedir um nome para o arquivo e pronto, cabeçalho feito!
![novosh](https://raw.githubusercontent.com/EppurSiMu0ve/novosh/master/20200120-204430.avi.gif)

Baseado nos ensinamentos do mestre [Blau Araujo](https://www.youtube.com/watch?v=c-YNy9wf5gk)

# personalizando
Para deixar o cabeçalho mais a sua cara faça o seguinte:
- crie o arquivo <b>~/.config/novosh/config</b>
- conteúdo do arquivo:
------------------------------------------------------------------
Autor: User Dev<br>
Contato: user.dev@zzzmail.com<br>
Licença: GNU/GPL v2 & v3<br>
Editor: geany<br>
Diretório: /home/user/documents #obs: sem barra no final<br>

-------------------------------------------------------------------
O script novosh vai ler e carregar essas informações dentro do cabeçalho dos seus scripts.
Eles serão salvos no diretório especificado e serão aberto com o editor indicado.
