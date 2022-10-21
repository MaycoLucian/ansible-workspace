# ansible-workspace
Esse repositório do ansible contém playbook para configuração do ambiente de trabalho, será atualizado conforme novas necessidade de ferramentas. As configurações funcionam para Debian. 


## Steps

> Veja o playbook main.yaml e se todas task fazem sentido.

1. Para rodar o playbook é necessário que você tenha o ansible instalado, caso não tenha pode executa-lo usando a linha abaixo:
> antes de executar a instalação recomendo a a leitura da [documentação oficial](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) 
```bash
sudo apt update && sudo apt install ansible unzip git -y
```

2. Realize o clone desse repositório

3. Executando o playbook
```bash
#acesse o repositório clonado e dentro execue a linha abaixo
ansible-playbook main.yaml --ask-become-pass
```
>Note que o playbook roda como root, sendo assim o comando --ask-become-pass faz com que a senha seja solicitada no inicio da execução.
