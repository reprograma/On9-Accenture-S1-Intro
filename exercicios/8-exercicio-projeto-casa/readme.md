# Exercício de contribuição em um projeto onde você é colaboradora

- Se você já fez `fork` do repositório dessa a aula, então não precisa fazer de novo.

- Para relembrar como um fork pode ser realizado, você pode ver as intruções de outro projeto no arquivo [sobre forl](../../conteudo/sobre-fork.md)

- Este exercício para casa segue fluxo similar ao exercício da pasta [5-exercicio-projeto-aula](https://github.com/reprograma/On9-Accenture-S1-Intro). Você pode usá-lo como referência.

### Instruções
* Entrar na pasta 8-exercicio-projeto-casa e siga as instruções a seguir.
* Adicionar link para imagem, link para seu github e o seu nome em uma `<div>`, seguindo o modelo com as informações da Paula Allemand.
	* Use o link do seu github para colocar no ***href*** na tag `<a>`. (Ex: https://github.com/reprograma)
	* Use o link da imagem do seu avatar no github para colocar no ***src*** da tag `<img>`. Clique com o botão direito sobre a imagem do seu perfil no github e copie o endereço da imagem. (Ex: https://avatars2.githubusercontent.com/u/41296983?s=460&u=d69e452fb89212415aca4769125d7efb7fc52727&v=4)
    * Exemplo de como capturar o link da imagem:
      <img src="./readme-assets/endereco-imagem.png">

  * Adicione seu nome no ***alt*** da tag `<img>`

  Exemplo:

    **Antes:**

    ```
    <div class="container__aluna">
        <a href="#/seu-link-do-github" target="_blank">
            <img class="container__aluna-img" src="#/seu-link-da-foto" alt="">
        </a>
        <p>Seu Nome</p>
    </div>
    ```
    
    **Depois:**
    
    ```
      <div class="container__aluna">
        <a href="https://github.com/itsalle" target="_blank">
          <img class="container__aluna-img" src="https://avatars2.githubusercontent.com/u/41296983?s=460&u=d69e452fb89212415aca4769125d7efb7fc52727&v=4"
            alt="Paula Allemand">
        </a>
        <p>Paula Allemand</p>
      </div>
    ```

* Conferir essa alteração no navegador (Chrome).
	* *Comportamento esperado: ao clicar na sua foto, o link do seu github irá se abrir numa aba nova*

* Voltando para o Git Bash.
* `git diff`: verificar o que você alterou no código.
* `git status`: verificar o status (ATENÇÃO: aqui se certifique que você está na branch com seu nome)
* caso não esteja na branch com seu nome, lista todas as branchs `git branch -a`
* `git checkout branch-com-meu-nome-sobrenome`: acessar a branch com seu nome e sobrenome :)
* `git add index.html`: Adicionar as alterações para área de preparação.
* `git status`: verificar o status novamente.
* `git commit -m "adicionando foto e link de <seu nome> para Githbub"`: adicionar mensagem de ***commit***.
* `git push origin branch-com-meu-nome-sobrenome`: subir as alterações da sua branch para o seu repositório remoto.
* Verificar se as alterações foram atualizadas na sua branch lá no github (https://github.com/reprograma/On9-Accenture-S1-Intro)


* Ir para a aba ***Pull requests***
* Criar novo pull request ***Compare & pull request*** pelo github da reprograma verificando se está fazendo a solicitação da nome-sobrenome para a master
* *base: **master**    **<=**    compare: **nome-sobrenome***

---

#### Após todos ***pull request*** dessa aula serem aceitos, caso queria atualizar localmente seu repositório:
* No Git Bash, dentro deste repositório.
* `git checkout master`: voltar para a branch master
* `git pull origin master`: atualizar o repositório local
* Verificar no navegador (Chrome) se todas as atualizações vieram

---
#### Deletar sua branch após seu ***pull request*** ser aceito
* `git checkout master`: estar na branch **master** para remover sua branch
* `git branch -d nome-sobrenome`: deletar sua branch **nome-sobrenome**
  ```

---
#### Para ter este repositório no seu GitHub, existem 2 alternativas:
- Subindo como você subiu todos os seus projetos;
- Fazendo um ***fork*** pelo próprio repositório da Reprograma;

---
#### Subir esse repositório no seu github
* Criar um novo respositório no seu github https://github.com/new
* Copiar o link do repositório.
* `git remote add meuRepo https://github.com/<seuLogin>/<seuNovoRepositorio>.git`: adicionar o link remoto pelo Git Bash. (Como o remote origin já está linkado ao repositório da Reprograma, iremos adicionar o seu remote com outro nome). Obs: Nesse link acima, substituir `<seuLogin>` e `<seuNovoRepositorio>` com informações do seu login e seu repositório.
* `git commit -m "Exercício para casa" --allow-empty`: fazer um ***commit*** vazio, pois tudo já foi adicionado anteriormente e não há novas alterações
* `git push meuRepo master`: Subir esse repositório local no seu repositório do GitHub.

---
#### Fazendo um ***fork*** pelo próprio repositório da Reprograma
* Ir no repositório da Reprograma e clicar em ***Fork***
<img src="./readme-assets/fork.png">