# Comandos Git

### Comandos básicos Git e terminais

Neste ponto, busca-se a listagem de alguns comandos simples para uso dos terminais em geral, sem a distinção dos Sistema Operacional, apenas para fins de consulta futura e melhor memorização.

- ls/dir - serve para se localizar no sistema e visualizar as pastas existentes.

- cd espaço nome da pasta/diretório - serve para entrar no diretório descrito na frente do comando cd.

- cd / - leva para a base do diretório c.

- cd .. - retorna um nível nos diretórios.

- mkdir nome do diretório a ser criado - serve para criar diretórios e no nome à frente do comando mkdir será o nome do diretório criado. 

- del - deleta apnas os arquivos mas deixa o diretório/pasta intacta. 

- rmdir /s /q  rm -rf - serve para deletar diretórios, modo recursivo excluindo os arquivos constantes nos diretórios e o próprio diretório. 

- echo - printa na tela a palavra colocada na frente.

- echo  oie > oie.txt - neste caso o sinal > redireciona o fluxo de texto para um arquivo, sendo criado um arquivo oie.txt, com a mensagem oie.

- **mv** (nome da pasta/arquivo) **./**(outra pasta) - **mv** para mover, **./** do repositório atual, para a pasta que colocarmos na frente.

- TAB - autocompleta nome de pastas/arquivos.

- cls/clear ou Ctrl+l - limpam o terminal. 

- up arrow (seta para cima) navega entre os comandos já utilizados, pode poupar tempo. 

### Comandos próprios para navegação no Git

Doravante, passo a listar os comandos específicos para utilização e navegação plena por intermédio dos comandos manuais do Git utilizando Git Bash.

Para adiantar o processo é possível navegar pela interface comum do PC até a pasta que se pretende trabalhar, clicar com o botão direito do mouse e dar um "git bash here" para já iniciar o programa diretamente na pasta desejada.

- git config --global user.email "descreva o e-mail" / git config --global user.name "descreva nome de usuário" - são comandos iniciais para configurar o git e fornecer autor e e-mail a nível global (para todos os projetos Git)

- git config --global --unset user.email / git config --global --unset user.name - para resentar e-mail e nome no git, sendo possível utilizar o comando anterior para estabalecer novo e-mail ou nome.

- git --list - para ver as configurações do seu git.

- git init - inicia um repositório git, possibilitando de fato um versionamento e gerenciamento do código pelo Git. o repositório em questão por padrão é nomeado como ".git", sendo, assim, uma pasta oculta por iniciar com "."

- ls -a - mostra as pastas ocultas.

- git add + nome da pasta - move arquivos para área de staged, possibilitando posterior commit (desta forma todo arquivo modificado dentro do git precisa ser apontado por nós ao sistema atrevés deste comando, para que ele comprrenda as modificações, gere novo SHA, modifique o status destes arquivos).

- git add * ou . - move todos os arquivos de modificação para staged, ficando prontos para serem commitados. 

- git commit -m "mensagem" - cria um commit e o -m "permite fazer uma anotação para esclarecer o conteúdo do commit"

- git status - possibilita monitorar os status dos arquivos 

- git clone +URL - baixa códigos do GitHub para sua máquina para que possa usá-lo por meio do git.

### Comandos conjuntos ao GitHub

Para criar o repositório no GitHub (repositório remoto) é necessário criar um novo repositório pelo GitHub. Este repositório será vazio, sendo necessário ir até nosso repositório local (Git) e apontar o repositório remoto do GitHub.

- git remote add origin +URL do repositório GitHub - aponta seu repositório local para o repositório do GitHub.

- git remote -v - lista os repositórios remotos cadastrados neste trbalho.

- git push origin main (ou master) - empurra a versão do repositório local para o repositório remoto

### Caso de conflito de códigos

Quando você faz uma alteração em seu código e na hora de fazer o push para o repositório remoto ocorre um erro, muito provavelmente será por existir conflito em nas mesmas linhas de códigos. Essa identificação de versões distintas será feita pela sua máquina, entretanto será necessário puxar (pull) o arquivo do repositório remoto para sua máquina para que você manualmente faça as alterações necessárias para que depois disponibilize a versão mais atual no GitHub. Esse acontecimento pode ser chamado de conflito de merge.

- git pull origin master (ou) main - puxa os arquivos do repositório remoto para sua máquina.

Posteriormente podemos seguir com os procedimentos comuns: git add, git commit e o push para o GitHub. 


