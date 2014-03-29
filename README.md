Moodle Novo Unb
===============

Script que baixa automaticamente arquivos do novo moodle da unb (http://ead.unb.br)


ATENÇÃO!
--------

Este script está porcamente comentado, é muito pouco verboso (isto é, não informa
ao usuário o que está ocorrendo) e baixa mais coisas do que o esperado. Porém funciona!

Espero corrigir bugs futuramente.

Se você sabe a programar em shell script e conhece bastante sobre Espressões Regulares, por
favor informe quaisquer bugs que você encontrar em melhorar o código. Se quiser pode me mandar
um email que te adicionarei como colaborador do script.

Este script só funciona para o novo [Moodle][] da UnB. Em breve criarei um script para o antigo
Moodle.

[Moodle]: http://ead.unb.br

Instalação
----------

1. Antes de instalar o script, verifique se você possui instalado os programas `lynx`, `bash` e `coreutils`

2. Para instalar o programa basta ter os dois arquivos `moodlenovo` e `moodlenovoget` num mesmo diretório.
Certifique-se de que ambos os arquivos sejam executáveis!

3. Crie no diretório `~/.config/` um arquivo chamado `moodlenovo.conf` e coloque nele duas variáveis em shell
que contém o nome do seu usuário (usualmente seu CPF) e a sua senha. Faça da seguinte forma:

``` bash
user=02578345321
passwd=1234
```

4. Entre no diretório para o qual deseja que os arquivos sejam baixados usando `cd` e execute nesse diretório
o scrip `moodlenovo`.


Nota
----

Este script se baseia em usar keybindings do browser `lynx` para mover pelo site da ead e expressões regulares
para obter no site a URL dos arquivos.

O arquivo `moodlenovo` apenas chama o `moodlenovoget` e esconde os processos realizados pelo lynx. Se deseja
ver o lynx trabalhando, então execute o `moodlenovoget`


Contato
-------

Lucas "Seninha" de Sena: `eu AT seninha.net`

