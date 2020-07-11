# Tutorial Transferência Repositórios

Tutorial de como fazer a transferência de um repositório do Bitbucket para o GitHub.

Primeiro de tudo é preciso criar o novo repositório no GitHub. Tenha o cuidado de desmarcar a opção "Initialize this repository with a README" enquanto cria o repositório. Dessa forma, o GitHub vai criar um repositório totalmente vazio.

Depois, copie a URL do repositório criado. Dentro da pasta onde você já possui o projeto hospedado no BitBucket clonado, execute os seguintes comandos:

```
$ git remote rename origin bitbucket
$ git remote add origin <URL do repositório criado>
$ git push origin master
```

Pronto! Todo o repositório do BitBucket vai ser copiado para o GitHub, inclusive mantendo o histórico de commits. 

Se desejar remover totalmente o projeto do BitBucket, execute também:

```
$ git remote rm bitbucket
```
