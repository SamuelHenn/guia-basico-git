# Guia básico sobre Git

## O que é o Git

O Git é um dos sistemas de **controle de versão** mais utilizados no mundo de desenvolvimento de software;

Isso significa que qualquer desenvolvedor numa equipe pode gerenciar o código-fonte e seu histórico de mudanças;

É gratuito e com o código fonte aberto;


## Porque usar?

O Git pode ser usado em todo e qualquer projeto que tenha arquivos de diferentes tipos, podendo ser código, texto, imagens, vídeos, áudios, entre outros;

Desempenho / Segurança / Flexibilidade;

Compartilhar e organizar o código entre o time de desenvolvimento;

Backup e facilidade em reverter alterações;


## Interfaces usadas

São ferramentas para hospedar os respositórios;

Facilitam a visualização do repositório;

Agregam funcionalidades;

Podem ter custos;

- GitHub - Muito usado no "mundo open source"
- GitLab - Tem mais recursos de CI/CD e gerenciamento de tarefas
- GitBucket - Tem mais recursos de CI/CD e gerenciamento de tarefas


## Instalando

### Linux 

```bash
	sudo apt-get install git-all
```

### Windows

- [Exe padrão para instalação](https://github.com/git-for-windows/git/releases/download/v2.35.1.windows.2/Git-2.35.1.2-64-bit.exe)


## Agora vamos ver as principais funções na prática


### Criar um repositório

* Crie uma conta no [GitLab](https://gitlab.com/users/sign_in)

* Crie um projeto

* Observação: É possível usar o Git apenas localmente na máquina, mas o normal é que fique hospedado em algum serviço.


### Clonar o repositório


Cria uma cópia de trabalho local do projeto;

* Abra o terminal
* Navegue até a pasta desejada
```bash
	git clone URL_DO_REPOSITÓRIO
```
* Informe usuário e senha


### Criar uma branch de trabalho

#### O que é uma branch

Branch significa “ramo”, ou seja, uma ramificação do seu código;

É usado para fazer modificações no código, sem afetar o código principal;

Representação gráfica:
![Branches](https://lh4.googleusercontent.com/hDZ7C2NQmOEeApDyPXFfjEfJyyIcmI8AfA8m-8loF8I2QKNrn4_Mw_IQKzoyj7O6SoKi2h6vTrKwZV5GL2uTJKSx_Kz8hSEpLAuhp7R_kpUYlW4H0oQbM34zo3fOZDtFU2PPtPr3)


#### Comandos

- Lista as branches existentes: ```git branch```

- Criar uma nova branch: ```git checkout -b NOME_DA_BRANCH```

- Mudar de branch: ```git checkout NOME_DA_BRANCH```


### Status

- Lista os arquivos que foram modificados: ```git status```


### Add

- Adiciona os arquivos modificados para serem comitados

	- Todos: ```git add .```


	- Por arquivo: ```git add CAMINHO_DO_ARQUIVO```

### Commit

Registra/salva as modificações que foram incluídas no 'add'


- Fazer o commit: ```git commit -m "Mensagem descrevendo o commit"```

