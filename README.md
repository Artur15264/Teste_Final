<h1> <b> Teste Final </b> </h1>

<h2> <b> Descrição do projeto: </b> </h2>

Ultimo item do cronograma de treinamento.<br />
Desenvolver um programa em C++ para printar Hello World, sem usar IDE, nem VSCode, tudo pelo terminal do Linux, apenas usando o editor de texto padrão (**nano**).<br />
O intuito desse projeto é testar os conhecimentos para criar diretórios e arquivos, editar arquivos, compilar, etc.

<h2> <b> Sobre o código: </b> </h2>

Consiste em um arquivo main.cpp que foi editado diretamente pelo terminal do Linux utilizando o nano.

Cada uma das etapas de desenvolvimento foram registradas e estão descritas abaixo, desde a criação do diretório até a atualização no Github.

<b> Etapas do projeto: </b>

- Inicializando o Git
- Criando o arquivo principal
- Editando o código
- Commit das alteraçoes
- Compilando e executando
- Enviando as aterações para o GitHub
- Aceitando o pull request no GitHub
- Atualizando o repositório local

---

<h2> <b> Inicializando o Git: </b> </h2>

Antes de iniciar a configração do git criei o diretório Teste_Final e apontei como diretório de trabalho atual com o comando `mkdir Teste_Final && cd Teste_Final` <br />
Apos isso pronto, foi a hora de criar o primeiro arquivo **README.md** e inicar o git no diretório utilizando o comando `git init` <br />
Com o git iniciado era hora de realizar o primeiro commit e realizar o push para o GitHub, com a sequencia de comandos abaixo:
- `git add .` -> Adiciona o conteudo que foi alterado
- `git commit -m "README.md"` -> Aplica as mudanças ao diretório oculto .git
- `git branch -M main` -> Altera o nome da branch para main, por padrão o nome é master
- `git remote add origin git@github.com:Artur15264/Teste_Final.git` -> Aponta o repositório local para um diretório remoto
- `git push -u origin main` -> Envia as alteraçoes do repositório local para o repositório remoto

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:

<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/7bc16a48-9796-470e-983f-090ab003b8d1">
</p> <br />

---

<h2> <b> Criando o arquivo principal: </b> </h2>

Para realizar alguma mudança no projeto é importante criar uma nova branch, nesse caso criei uma branch chamada desenvolvimento, onde criei o arquivo main.cpp e realizei todas as alteraçoes.<br />
O comando `echo` pode ser usado para criar novos arquivos utilizando o complemento `>>` seguindo a sequencia de comandos abaixo:
- `git branch desenvolvimento .` -> Cria a branch desenvolvimento
- `git checkout desenvolvimento"` -> Altera para a branch desenvolvimento
- `echo "// Hello World em C++ >> main.cpp"` -> Cria o arquivo main.cpp com o texto **// Hello World em C++**
- `nano main.cpp` -> abre o arquivo main.cpp no **nano**, editor de texto do Linux pelo terminal

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:

<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/0c0f1f26-0242-43a1-b79b-1a5459fccf32">
</p> <br />

---

<h2> <b> Editando o código: </b> </h2>

O código foi escrito direto pelo nano, após o código pronto foi necessário salvar e sair do nano para aplicar as alterações.

A imagem abaixo mostra o código escrito no nano:

<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/23bf48d9-7365-476d-9345-47de07346ce8">
</p> <br />

---

<h2> <b> Commit das alteraçoes: </b> </h2>

Apos a alteração do codigo é necessario adicionar essa mudança ao git com `git commit`<br />
Abaixo está a sequencia de comandos utilizados:
- `ls` -> Lista os arquivos e diretórios presentes dentro de um diretório
- `git status` -> Mostra os arquivos que ainda não foram adicioandos usando o **git add**
- `git add` -> Adiciona o conteudo que foi alterado
- `git commit` -> Aplica as mudanças ao diretório oculto .git

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:

<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/f500d6b3-1f54-450c-bfc4-ab4a5d7a9523">
</p> <br />

---

<h2> <b> Compilando e executando: </b> </h2>

Para compilar utilizei o próprio compilador do Linux, o GCC(GNU Compiler Collection) é um compilador para vários tipos de arquivos, como esse projeto é em C++ foi necessário utilizar o g++ para compilar <br />
Para executar o programa via terminal é necessário usar `./Nome-do-Arquivo` <br />
Abaixo está a sequencia de comandos utilizados:
- `ls` -> Lista os arquivos e diretórios presentes dentro de um diretório
- `g++ -g -o HelloWorld main.cpp` -> mostra os arquivos que ainda não foram adicioandos usando o **git add**
- `ls` -> Lista os arquivos e diretórios presentes dentro de um diretório
- `./HelloWorld` -> Adiciona o conteudo que foi alterado

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:

<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/ae5e0b2c-ab8a-4843-ae1e-c6558082c30a">
</p> <br />

---

<h2> <b> Enviando as aterações para o GitHub: </b> </h2>

Antes de enviar as alteraçoes para o GitHub é necesário realizar o processo de `add` e `commit` <br />
Nesse ponto usei o comando `git log` para mostrar a diferença de log na branch **desenvolvimento**, onde foram feitas as alteraçoes, e a branch **main**. <br />

A imagem abaixo mostra o log na branch desenvolvimento:
<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/5e47ab41-112d-4e7a-a044-ea0c17b9898e" >
</p> <br />

Para enviar as alterações para o GitHub primeiro é necessário alterar da branch **desenvolvimento** para a branch **main** utilizando o comando `git checkout` <br />
Após isso, é possivel enviar as mudanças utilizando o comando `git push` <br />
Abaixo está a sequencia de comandos utilizados:
- `git checkout main` -> Troca da branch desenvolvimento para a branch main
- `git pull origin main` -> Baixa os arquivos da branch main que estão no GitHub para manter o projeto atualizado
- `git push origin desenvolvimento` -> Envia a branch desenvolvimento para o GitHub
- `ls` -> Lista os arquivos e diretórios presentes dentro de um diretório
- `git log` -> Mostra o registro de commits que foram realizados até o momento

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:
<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/ab4861a5-d622-414b-a04f-90a4c2abf7b9" >
</p> <br />

---

<h2> <b> Aceitando o pull request no GitHub: </b> </h2>

Esta etapa foi realizada dentro do GitHub, consiste em aceitar o pull request que foi criado na etapa anterior e realizar o merge da branch desenvolvimento, na branch main <br />
Não foi utilizado nenhum comando nesta etapa do projeto. <br />

<p align="center">
  <b> A imagem abaixo mostra a página inicial do projeto antes de realizar o pull request: </b>
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/7aac683e-02c7-4075-9813-664082bdb679">
</p> <br />

<p align="center">
  <b> As imagens abaixo mostram o processo de pull request: </b>
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/573ab9df-dcd7-427b-87f9-1d11ceb61487" >
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/d4d22e35-104c-4c5e-8e56-fbc313b82114" >
</p> <br />

<p align="center">
  <b> A imagem abaixo mostra a página inicial durante o merge: </b>
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/5205ea89-95cc-4ea4-aad7-83c02b4331ee">
</p> <br />

<p align="center">
  <b> A imagem abaixo mostra a página inicial do projeto depois de realizar o merge: </b>
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/df77408c-a6ce-45a9-847e-8097b83608a4">
</p> <br />

---

<h2> <b> Atualizando o repositório local: </b> </h2>

Apos realizar as alteraçẽs no GitHub é necessário atualizar o repositório local com o comando `git pull`
Abaixo está a sequencia de comandos utilizados:
- `git log` -> Mostra o registro de commits que foram realizados até o momento (incompleto)
- `git pull origin main` -> Baixa os arquivos da branch main que estão no GitHub para manter o projeto atualizado
- `git log` -> Mostra o registro de commits que foram realizados até o momento (completo)

A imagem abaixo mostra a sequencia descrita acima no terminal do Linux:
<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/6b84a44f-9261-4daf-8b53-9cd221e1be05">
</p> <br />

A imagem abaixo mostra como ficou o log final e mostra um teste para verificar se todos os arquivos foram importados do GitHub executando o programa de novo:
<p align="center">
  <img  width="819" height="517" src="https://github.com/Artur15264/Teste_Final/assets/153198439/1b219099-c5e5-44ac-8698-956fe4fb4b18">
</p> <br />


