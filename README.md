# bandtec-2-semestre-Dev
# Documenta��o do Projeto

## Indice

* Ferramentas para diagramas
* Regras para organiza��o dos reposit�rios
* Comandos relacionados a branch
* Comando �teis do git
* Diferen�a entre Merge e Rebase
* Extra

---
## Ferramentas para diagramas
- (DIAGRMAS EM GERAL) https://www.lucidchart.com/pages/
- (BPMN) https://www.bizagi.com/en/products/bpm-suite/modeler
- (DIAGRAMAS EM GERAL) https://pencil.evolus.vn/

### Regras para organiza��o dos reposit�rios

Quando realizar altera��o no git devemos dar o `git commit` e o `git push` para um **branch novo**.
Quando a edi��o realizada no branch estiver completa deve ser feito um **push request** no GitHub e dois dos desenvolvedores devem checar as altera��o para ver se existe conflito e verificar o c�digo para que ele seja fundido (merge) com o branch master.

### Comandos relacionados a branch:
- `git branch` = mostra todas as branchs existentes

-`git branch -a` - mostra os branchs locais e os remotos (que est�o no github)

- `git checkout -b NOME-DO-BRANCH` = Cria uma nova branch - a partir da branch **master**.

- `git checkout NOME-DO-BRANCH` = sem o `-b` o comando troca de branch

- `git push -u origin NOME-DO-BRANCH` = D� o push para a nova branch.

- `git branch -d NOME-DO-BRANCH` = Deleta o branch.

- `git merge NOME-DO-BRANCH` = Pega o cont�udo do branch desejado e passa para o branch atual.

---

### Comando �teis do git

- `git commit --amend --no-edit --author "NOME CERTO <emailcerto@mydomain.com>"` = Se deu commit com nome/email errado 

- `git commit -am "coment�rio objetivo"` = Permite voc� j� adicionar arquivo no 'palco' (stage) para que possam ser dado um commit direto.

- `git commit --amend` = Sobrescreve o �ltimo commit.


- `git commit --amend -C HEAD` = Adiciona ao ultimo commit com o mesmo coment�rio.

- `git revert ID-DO-COMMIT` = Reverte o conte�do e volta as altera��es do commit.

*Exemplo: `git revert 504fab770bf8e892ce9a56c6a3fb85eec5320cdf`*.

- `git checkout NOME-DO-ARQUIVO` = Reverte o arquivo para seu estado anterior.

- `git checkout --.` = Reverte tudo.

### Diferen�a entre Merge e Rebase

O **merge** mescla o *branch* atual com *outro branch* ambos em seu estado atual.
O **rebase** pega seu *branch* atual e muda seu inicio, sua base.


### Extra

Site que te ajuda achar mais facilmente comandos do git: [git_explorer](https://gitexplorer.com/).


**Sites �teis**
- https://github.com/k88hudson/git-flight-rules
- https://github.com/bennadel/git-cheat-sheet

