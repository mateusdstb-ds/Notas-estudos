## Configurando chave ssh git hub

```js 

1-Como primeiro passo você deve abrir a aba pesquzar do seu computador ou Nootbook .

2-Feito isso você precisara digitar CMD ou Terminal de Comando.Feito isso abra-o.

3-Digitar o comando ```js git --version ``` isso fara com que aparecerá a verção do seu git . Caso seu git estiver desatualizado estando abaixo de 2.53.0
atualize seu git pelo google .

4- Agora você vai salvar seu nome e seu email no CMD  usando esses dois comandos>

```js
git config --global user.name “Seu Nome”

git config --global user.email “seuEmail@gmail.com”

```
O esse gmail precisa ser o mesmo que você usou no github .

5-Agora vamos para o git bash  com a instalação do git o git bash automaticamente ja será instalado 

Vamos verificar se você ja possui uma chave ssh dentro da sua maquina  usando o comando ```js ls -al ~/.ssh``
caso não tenha otimo vamos iniciar e adicionar uma chave com esse comando 
```js  ssh-keygen -t ed25519 -C “your_email@example.com” ```

Depois vamos inicializar agente
```js eval "$(ssh-agent -s) ```

agora vamos adicionar a chave ao agente 
````js ssh-add ~/.ssh/id_ed25519 ```

Agora por ultimo vamos copiar a chave 

```js  clip < ~/.ssh/id_ed25519.pub ```



