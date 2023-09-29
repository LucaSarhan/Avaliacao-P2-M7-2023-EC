# Template para avaliação P2

Saída esperada após execução do programa:

<img src="./media/tela-front.png" display="flex">

# IMPORTANTE:

Para colocar o frontend para funcionar, colocar uma máquina EC2 rodando o Apache WebServer.
Para isso, instalar dentro da EC2:

```bash
sudo apt update
sudo apt upgrade
sudo apt install apache2
# os arquivos do projeto devem estar em /var/www/html
git clone https://github.com/Murilo-ZC/Avaliacao-P2-M7-2023-EC.git
sudo cp ./Avaliacao-P2-M7-2023-EC/frontend /var/www/html
```

Aqui pessoal, os arquivos já estaram disponíveis na porta 80, não necessário redirecionar.

> IMPORTANTE: Verificar as rotas e utilziar o seu próprio repositório com as modificações realizadas.

# Relatório da prova
Segue o [link](https://docs.google.com/document/d/1Qd2RWp6XjU82leSxHrZPTcZlCuJB-cRt6MRWa-I-fkY/edit?usp=sharing) das imagens que comprovando o que foi feito na AWS.
Primeiro eu criei a instância do EC2 do front na prova. Foi selecionado o ubuntu como o sistema operacinal, todas as regras de trafego(SSH, HTTP e HTTPS) foram ligados, uma regra de entrada na parte de segurança foi adcionado para permitir connectar com qualquer lugar IPV4. Foi criado um key pair para acessar a instancia. Depois seguir todos os comandos acima no terminal do EC2. Depois seguir em fazer o RDS da atividade onde foi selecionado o postgres como banco de dados e nome do usuario e a senha foi escolhida com admin123. Depois testei a connexão do RDS com o DBeaver que confirmou a connexão. O mesmo processo de criação da EC2 do frontend foi repetido para a instância do backend. 
