# Aprendendo Git e Github
> Estou usando este repositório para aprender Git e Github, os arquivos não contém projetos reais, são apenas ilustrações.

### Trabalhando em um repositório de forma offline
* Primeiramente você precisa ter o git instalado no seu pc: https://git-scm.com/
* Com o Git instalado, você deve uma escolher uma pasta no seu PC para armazenar o projeto, apertar com o botão direito do mouse nela e clicar em 'Git Bash Here'.
* Após isso, irá abrir o prompt de comando do Bash.
* Agora você deve voltar ao GitHub e abrir o repositório que deseja trabalhar no seu PC.
* Clique no botão `<> Code` e copie o link `https` que aparecer.

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/7672d942-63bd-4cec-872a-6ad4962ca9c1)

Após copiado o link, você deve voltar ao terminal e digitar o seguinte comando:
` git clone link `
> No lugar de link, você cola o link que você copiou. O comando de colar pode variar, dependendo do sistema operacional utilizado. Para mim, que uso o Windowns 10, funciona apenas clicar com o botão direito do mouse, que ele já cola automaticamente.

* Após executar o comando, se tiver dado tudo certo, você já tera a cópia do projeto no seu PC.
* Agora basta você abrir o projeto na sua IDE e já estará pronto para editá-lo.

![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/5c4f351d-292b-4f04-a011-8781550965ee)

* Após feita as alterações, você pode fazer o `commit` e o `push` para salvar suas atualizações no GitHub.
* Para isso, você deve voltar ao `terminal do bash` e coloca-lo para operar na pasta do projeto.

Existem 3 formas de fazer isso:

1. Você pode usar o comando `cd nome-da-pasta`.
![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/4c969c29-ac28-4e79-8c91-5e7fe8e4a45b)

2. Você pode fechar o terminal e abri-lo novamente diretamente na pasta, usando o mesmo processo ensinado anteriormente (Git Bash Here).

3. Você pode abrir o Bash no próprio VScode, selecionando-o nas opções de terminais:
![image](https://github.com/thiagoreys/sistema-de-cadastro/assets/130335096/567f02af-b1b3-459d-994f-e3e311ae0ae4)

Após colocado o Bash para operar diretamente na pasta do repositório, você deve digitar os seguintes comandos.
```
git commit . -m "mensagem de commit"
git push
```
> Obs: os comandos devem ser executados na mesma sequência.

Pronto, feito tudo corretamente, os arquivos já estaram atualizados no seu GitHub.

