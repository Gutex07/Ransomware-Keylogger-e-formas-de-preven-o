# Ransomware - Keylogger e formas de prevenção
Atenção: este repositório é destinado apenas a fins educacionais, de defesa e pesquisa em segurança. Não contém código malicioso, nem instruções para criação de malware. Qualquer experimento deve ser feito em ambientes isolados (máquina virtual), com autorização e respeitando as leis e políticas locais.

## Projeto: Análise e Simulação (Segura) de Ameaças — Ransomware & Keylogger (Documento Técnico)

Este projeto documenta, de forma não-executável e didática, conceitos, fluxos de ataque e medidas de proteção relacionadas a duas classes de ameaças: ransomware e keyloggers. O objetivo é servir como material de referência para:

Profissionais de segurança;
Instrutores e estudantes em cursos de cibersegurança;
Administradores que querem entender vetores e mitigações.

O repositório não contém código perigoso. 
Contém: explicações conceituais, cenários de teste seguros (com artefatos não-maliciosos), guias para montar laboratórios isolados, e recomendações de detecção e resposta.

---
## Implementação do Ransoware

1 etapa - importar as bibliotecas 1 para criptografar (Fernet) os dados e outra para navegar pelas pastas da vítima e encontrar os arquivos (os).

2 etapa - Inicia a criação do código ransoware com uma função para criar e salvar uma chave de criptografia. Uma chave que vai transformar os dados legíveis e m informações criptografadas e retorná-los ao normal.

3 etapa - criar uma função para guardar a chave criada e depois ser utilizada no processo de criptografia.

4 etapa - criar uma função para criptografar o arquivo original e sobrescrever o conteúdo do arquivo com os dados criptografados.

5 etapa - criar função para encontrar e capturar os arquivos dentro do computador da vítima. Excluir dessa busca o próprio malware para não criptografar o próprio vírus.

6 etapa - criar a função de resgate para enviar a vitima as instruções  do dano e as formas de recuperar o acesso aos dados.

7 etapa - criar a função principal para executar todos os passos do código em sequência. Gerar a chave, carregar a chave, encontrar os arquivos, criptografar todos e criar a mensagem de resgate. E ao final a mensagem de êxito do código.

8 etapa - Uma linha final para garantir que se o script for executado corretamente a função main será executada.
