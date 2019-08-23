# Documentação do Projeto

## Indice

* Regras para organização dos repositórios

---

### Regras para organização dos repositórios

Quando realizar alteração no git devemos dar o `git commit` e o `git push` para um **branch novo**.
Quando a edição realizada no branch estiver completa deve ser feito um **push request** no GitHub e dois dos desenvolvedores devem checar as alteração para ver se existe conflito e verificar o código para que ele seja fundido (merge) com o branch master.


#### Comandos relacionados:
- `git branch` = mostra todas as branchs existentes

- `git checkout -b NOME-DO-BRANCH` = Cria uma nova branch - a partir da branch **master**.

- `git push -u origin NOME-DO-BRANCH` = Dá o push para a nova branch.

- `git branch -a NOME-DO-BRANCH` = Deleta o branch.

- `git merge NOME-DO-BRANCH` = Pega o contéudo do branch desejado e passa para o branch atual.

### Comando úteis do git

- `git commit -a -m "comentário objetivo"` = 

- `git commit --amend` = Sobrescreve o último commit.

- `git revert ID-DO-COMMIT` = Reverte o conteúdo e volta as alterações do commit.

*Exemplo: `git revert 504fab770bf8e892ce9a56c6a3fb85eec5320cdf`*.

- `git checkout NOME-DO-ARQUIVO` = Reverte o arquivo para seu estado anterior.

- `git checkout --.` = Reverte tudo.

### Diferença entre Merge e Rebase

O **merge** mescla o *branch* atual com *outro branch* ambos em seu estado atual.
O **rebase** pega seu *branch* atual e muda seu inicio, sua base.


