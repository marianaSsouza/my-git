# Testando e resolvendo conflito!
## ~ início
- Primeiro, criei uma branch chamada feat/resolvendo-conflitos

<br>
![print criando branch]("\imagens_my-git\criando-branch-resolvendo-conflito.png")
<br>

- Após isso, criei um arquivo no repositório <u><strong>my-git</strong></u> chamado <u><strong>resolvendo-conflitos.md</strong></u>
- nele fiz algumas alterações e fiz um commit seguindo o fluxo
> git add .
<br>
 git commit -m "teste"
 <br>
 git push

- depois, troquei de branch com o comando <u><strong>git checkout main</strong></u> e comecei a testar
---
### ~ conflito
- para esse conflito, primeiro fiz uma alteração no meu repositório remoto no github e dei um commit por lá mesmo
<br>
adicionar imagem!!

- no meu repositório local, eu também fiz uma alteração na minha branch main, na mesma linha onde fiz a alteração remota. Para mudar de branch, segui o comando <u><strong>git checkout main</strong></u>
- como eu ainda não tinha dado pull na alteração remota e já fui direto fazer a alteração local, o comando <u><strong>git status</strong></u> mostrou o seguinte:

<br>

adicionar imagem git-status-mesagem.png

- a seguir, joguei essa alteração para stage com um <u><strong>git add .</strong></u> e commitei ela com <u><strong>git commit -m "testando conflito na main</strong></u>

- porém, quando fiz esse commit, gerou um conflito:
<br>
adicionar imagem conflito-01-git

---
### ~ como resolvi:

- segui o comando <u><strong>git pull</strong></u> para trazer as alterações do remoto para o meu local
- logo quando dei esse git pull, apareceu a seguinte mensagem:

<br>
adicionar a imagem escolhendo-alteracoes

- após escolher a opção que gostaria (no meu caso escolhi a atual), segui com o comando:
> git status
<br>
> git add . && git commit -m "teste" && git push

- o que gerou a saída:

adicionar imagem saida-do-git-pull

- resolvendo assim o conflito :)










