# notas-estudo
minhas notas de estudo do téc SENAC 2026

markdown 


## configurando Git:

para utilizar o Git na minha maquina eu preciso configurar determinado comandos , sendo eles: Git --version para verificar se o git esta instalado, 

'''bash 
git config --global 
'''
## como configurar Github :
use os comados: Git config --global user.name "seu nome"
 Git config --global use.email "seuemail@gmail.com"

## SSH - Como configurar a maquina para GitHub :
verificar se existe chave ssh.
adicionar uma nova chave 
ssh-keygen -t ed25519 -c "your_email@exemple.com"
iniciar agente-ssh
eval "$(ssh-agent-s)"
adicione chave ssh no agente.
 ssh-add -/ssh/id_ed25519

## como criar um repositório :
entre no GitHub, vá em repositório aperte no botão "new" coloque um nome e uma descrição no repositorio e ative o README 
