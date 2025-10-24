# Ransomware - Keylogger e formas de prevenção
Atenção: este repositório é destinado apenas a fins educacionais, de defesa e pesquisa em segurança. Não contém código malicioso, nem instruções para criação de malware. Qualquer experimento deve ser feito em ambientes isolados (máquina virtual), com autorização e respeitando as leis e políticas locais.

---
## 🦠 Ransoware

- Importar as bibliotecas 1 para criptografar (Fernet) os dados e outra para navegar pelas pastas da vítima e encontrar os arquivos (os).
- Inicia a criação do código ransoware com uma função para criar e salvar uma chave de criptografia. Uma chave que vai transformar os dados legíveis e m informações criptografadas e retorná-los ao normal.
- Criar uma função para guardar a chave criada e depois ser utilizada no processo de criptografia.
- Criar uma função para criptografar o arquivo original e sobrescrever o conteúdo do arquivo com os dados criptografados.
- Criar função para encontrar e capturar os arquivos dentro do computador da vítima. Excluir dessa busca o próprio malware para não criptografar o próprio vírus.
- Criar a função de resgate para enviar a vitima as instruções  do dano e as formas de recuperar o acesso aos dados.
- Criar a função principal para executar todos os passos do código em sequência. Gerar a chave, carregar a chave, encontrar os arquivos, criptografar todos e criar a mensagem de resgate. E ao final a mensagem de êxito do código.
- Uma linha final para garantir que se o script for executado corretamente a função main será executada.
---
## ☣️ Keylogger
O logger será executado em segundo plano, toda vez que o usuário digitar uma tecla o programa vai capturar essa informação e gravar em um arquivo .txt. Em seguida, o arquivo irá apresentar todas as informações capturadas de forma sequencial.

---

- Criação do código keylogger incluindo a biblioteca necessária (pynput), para capturar as teclas e em seguida configurando os parâmetros referente quais as teclas serão ignoradas e quais serão as teclas capturadas pelo logger.
- Em seguida com a execução do Keylogger, ele começa a registrar em um arquivo txt tudo que a vitima digita no seu computador.
- Tornando o keylogger mais camuflado ao usuário. Alterando a extensão do arquivo de py para pyw, são scripts python que rodam em segundo plano no Windows. Logo após a alteração da extensão o keylogger vai rodar em segundo plano e capturando as teclas que o usuário digitar.
- Enviar os dados remotamente par ao atacante. A automatização do envio dos dados da vítima para o atacante é possível ser realizadas configurando o e-mail (criado para fins de estudo) com a verificação de 2 etapas para conectar com o python.
- Dentro do código python do keylogger fazer a instalação das bibliotecas necessárias para enviar o e-mail. (smtplib)formatar as teclas capturadas como mensagem de texto (email.mine.text) e a biblioteca que vai permitir configurar o intervalo do envio das informações (Timer). Em seguida durante a criação do código inserir as informações do e-mail criado para receber as informações capturadas pelo keylogger.

---

## 🧪 Formas de proteção e prevenção

- Antivirús e firewall sempre atualizados e bem configurados;
- Ferramentas de segurança modernas para monitorar o comportamentos de programas e aplicativos;
- Conscientizar e treinar os usuários referente a prevenção de atitudes que podem abrir brechas no sistema para invasão de  software maliciosos, como e-mails duvidosos, compartilhar senhas e acesso a sites inseguros;
- Utilizar ambientes isolados para fazer testes, rodar códigos abertos. Sempre utilizar ambientes controlados para realizar teste e ajustes para não afetar todo o sistema. Exemplo máquina virtual (Virtual Box); e
- Compartilhar o conhecimento para outras pessoas pois a parte mais frágil e de maior acesso do sistema é o usuário. Portanto todo bom conhecimento de prevenção deve ser compartilhado entre os usuários do sistema para que todos saibam se prevenir dos ataques.

Reforçando que todo conhecimento e informações repassadas nesse projeto são para fins didáticos do curso de formação em Cybersecurity.
