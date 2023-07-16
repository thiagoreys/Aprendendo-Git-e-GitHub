# Aprendendo Git e Github
> Estou usando este repositório para aprender Git e Github, os arquivos não contém projetos reais, são apenas ilustrações.

## Trabalhando em um repositório de forma offline
* Primeiramente você precisa ter o Git instalado no seu pc: https://git-scm.com/
* Com o Git instalado, você deve uma escolher uma pasta no seu PC para armazenar o projeto do seu repositório.
* Após escolher a pasta, aperte com o botão direito do mouse nela e clique em 'Git Bash Here'.
* Após isso, irá abrir o prompt de comando do Bash.

![image](https://github.com/thiagoreys/Aprendendo-Git-e-GitHub/assets/130335096/b5f21784-37bd-4d22-84b0-89b23e69b001)

* Feito isso, agora você deve voltar ao GitHub e abrir o repositório que deseja trabalhar no seu PC.
* Clique no botão `<> Code` e copie o link `https` que aparecer.

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/7672d942-63bd-4cec-872a-6ad4962ca9c1)

Após copiado o link, você deve voltar ao terminal e digitar o seguinte comando:
` git clone link `
> No lugar de 'link' você cola o link que você copiou. O comando de colar pode variar dependendo do sistema operacional utilizado. Para mim, que uso o Windowns 10, funciona apenas clicar com o botão direito do mouse, que ele já cola automaticamente.

* Após executar o comando, se tiver dado tudo certo, você já tera a cópia do projeto no seu PC.
* Agora basta você abrir o projeto em sua IDE e já estará pronto para editá-lo.

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/5c4f351d-292b-4f04-a011-8781550965ee)

## Atualizando o repositório no GitHub

Após feita as alterações, você pode fazer um `commit` e um `push` para salvar suas atualizações no GitHub. Para isso, você deve:

* Abrir o `Terminal Bash` e coloca-lo para operar na pasta do projeto.

Existem 3 formas de fazer isso:

1. Você pode usar o comando `cd nome-da-pasta`.

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/4c969c29-ac28-4e79-8c91-5e7fe8e4a45b)

2. Você pode fechar o terminal e abri-lo novamente diretamente na pasta, usando o mesmo processo ensinado anteriormente (Git Bash Here).

3. Você pode abrir o Bash no próprio VScode, selecionando-o nas opções de terminais:

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/567f02af-b1b3-459d-994f-e3e311ae0ae4)

Após colocado o Bash para operar diretamente na pasta do repositório, você deve executar os seguintes comandos:
```
git commit . -m "mensagem de commit"
git push
```
> Obs: os comandos devem ser executados na mesma sequência.

Pronto, feito tudo corretamente, os arquivos já estarão atualizados em seu GitHub.

## Atualizando o repositório na sua máquina

Caso já tenha o repositório salvo na sua máquina e queira apenas atualiza-lo para a sua versão mais recente disponível no GitHub, basta seguir os seguintes passos:

* Abra o `Terminal Bash` na pasta do repositório em seu computador.
* Digite o seguinte comando:
```
git pull link
```
> No lugar de link, você cola o link do repositório do GitHub.

E pronto, ao executar o comando, os arquivos do repositório serão atualizados em sua máquina local.

## Trabalhando em versões antigas de um repositório

Também existe a opção de você trabalhar em versões antigas de um projeto, para correção de bugs ou reformulação do projeto.
Para isso você deve abrir o repositório do projeto que deseja trabalhar no GitHub e clique em `commits`.

![image](https://github.com/thiagoreys/Aprendendo-Git-e-GitHub/assets/130335096/7aa1210d-e8ce-4d0e-9896-0506bfc3d2b3)

Lá você vai ter acesso a todos os `commits` do seu projeto.

![image](https://github.com/thiagoreys/Aprendendo-Git-e-GitHub/assets/130335096/4e0a08c1-5063-4c5b-9d9c-8d76be099e5f)

Caso queira trabalhar em cima de alguma dessas versões, copie o código `hash` do commit também conhecido como 'SHA'.

![image](https://github.com/thiagoreys/Aprendendo-Git-e-GitHub/assets/130335096/498a37b4-c542-4774-8475-f99ecc45075e)

Agora você deve abrir novamente o `Terminal Bash` na pasta em que deseja trabalhar e executar os seguintes comandos:

``` 
git restore --source codigohash .
```
> No lugar de 'codigohash' você deve colar o código `hash` do commit (botão direito do mouse).

Pronto, agora o repositório do projeto na versão selecionada já estará disponível para edição na sua máquina.

## Criando ramificações no projeto (Branchs)

Até o momento só trabalhamos com o projeto principal `main`, entretanto podemos ramificar o nosso projeto em branchs para `desenvolvimento` e `testes` por exemplo, o que é muito importante para organização de projetos maiores em que se trabalham equipes de desenvolvedores.

Para criar novos branchs, podemos digitar o seguinte comando no `terminal bash` do projeto:
```
git checkout -b branch
```
> No lugar de 'branch' digitamos o nome do branch que queremos criar.

Após rodar o prompt o diretório já é alterado para a `branch` criada.

![image](https://github.com/thiagoreys/Aprendendo-Git-e-GitHub/assets/130335096/13dcfffb-0f32-40cf-a113-387f8fa44efe)

Agora podemes adcionar atualizações na branch de `desenvolvimento` ao invés de diretamente no projeto principal `main`. Isso é importante para que o time de desenvolvimento possa fazer testes e analisar com cautela os novos códigos adcionados, para que assim o projeto corra menor risco de *bugs* e incompatibilidades.

Caso queira voltar para branch principal, basta digitiar o seguinte comando:

```
git switch main
```
