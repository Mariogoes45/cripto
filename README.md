# cripto

Este repositório contém um conjunto de scripts Python desenvolvidos exclusivamente para fins educacionais e de estudo. O projeto simula a funcionalidade básica de um ataque de ransomware (criptografia de arquivos) e sua respectiva ferramenta de descriptografia.

O objetivo principal é demonstrar a implementação de criptografia simétrica com a biblioteca cryptography.fernet e servir como um laboratório seguro para praticar a resposta a incidentes e o desenvolvimento de ferramentas defensivas (decryptors).

⚠️ Atenção: Este código não deve ser executado em ambientes de produção ou usado para atividades ilegais. O uso indevido é de total responsabilidade do usuário.

Tecnologias Utilizadas
Linguagem: Python 3.x

Criptografia: cryptography.fernet (Criptografia simétrica AES 128-bit, Fernet Specification)

Pré-requisitos
Ter o Python 3.x instalado.

Instalar a biblioteca cryptography:

Simular o Ataque (Criptografia)
O script ransoware.py irá: (1) Gerar uma nova chave em chave.key, (2) criptografar todos os arquivos na pasta test_files, e (3) criar o arquivo LEIA-ME.txt.

Crie uma pasta chamada test_files na raiz do projeto.

Adicione alguns arquivos (ex: documento.txt, foto.jpg) dentro de test_files.

Execute o script do "ransomware":

Bash

python ransoware.py
Verifique: Seus arquivos em test_files estarão criptografados, e um novo chave.key será gerado.

2. Simular a Descriptografia (Recuperação)
A simulação de recuperação requer a chave gerada. O script descriptografar.py utiliza essa chave para reverter o processo:

Certifique-se de que o arquivo chave.key (gerado pelo ransoware.py) está no mesmo diretório.

Execute o script de descriptografia:

Bash

python descriptografar.py
Verifique: O script irá ler a chave, descriptografar os arquivos em test_files e imprimir a mensagem de conclusão.
