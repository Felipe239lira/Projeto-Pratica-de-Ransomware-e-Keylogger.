    🚨 Projeto de Estudo: Ransomware em Python

![Imagem Futurista de Ransomware](https://copilot.microsoft.com/th/id/BCO.9491577b-c5dc-4b77-af09-354b0bdfa816.png)

Este projeto tem como objetivo **demonstrar de forma didática** como funciona um ransomware simples, utilizando a linguagem Python.  
⚠️ **Atenção:** O código aqui apresentado é apenas para fins educacionais e deve ser executado **somente em ambientes controlados**. Qualquer uso indevido é de inteira responsabilidade do usuário.

    🛠️ Estrutura do Projeto

- `encript.py` → Script responsável por criptografar arquivos em um diretório alvo.
- `decript.py` → Script responsável por descriptografar os arquivos utilizando a chave gerada.
- `README.md` → Documentação do projeto.
- `images/` → Pasta com imagens ilustrativas do processo (incluindo prints e diagramas).

      🔒 Como Funciona

1. O script gera uma chave de criptografia.
2. Os arquivos do diretório alvo são criptografados.
3. Uma mensagem de alerta é exibida (simulando instruções de resgate).
4. O script de decriptação tenta restaurar os arquivos utilizando a chave correta

  Segue abaixo fluxograma de como ira funcionar:

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/b1dc4d04-55bc-4046-b32e-f1669418fb31" />


       📷 Ilustrações

 Primeiro vamos importar as bibliotecas Fernet e os.

from cryptography.fernet import Fernet

import os      
  
  Criaremos a função para gerar a chave e a função para carregar a chave.

<img width="441" height="177" alt="image" src="https://github.com/user-attachments/assets/557c121c-2e94-42a5-b289-15dce23f27c0" />

Em seguida criaremos as funções para criptografar os arquivos e para encontrar o nosso diretorio alvo.

<img width="788" height="443" alt="image" src="https://github.com/user-attachments/assets/c838c745-c5a7-4154-9588-d9c17c1d28fe" />

Agora vamos criar a função que gera as instruções de pagamento

<img width="735" height="119" alt="image" src="https://github.com/user-attachments/assets/12e4fa20-3e61-4bbe-8b5e-761eebae5049" />

Seguimos criando a função principal do Ransomware e para dar uma graça vamos importar o modulo messagebox da biblioteca tkinter e criar uma menssagem de alerta ao criptografar os arquivos.

<img width="1063" height="410" alt="image" src="https://github.com/user-attachments/assets/82542a53-c4f6-4884-af9e-c50af9c2f414" />

    Executando o Ransomware
    
Verificando que nossos arquivos estão perfeitamente normais.

<img width="1337" height="465" alt="image" src="https://github.com/user-attachments/assets/4142c63c-b733-4599-9098-3422767f93e7" />

Ao executar nosso Ransomware ele apresenta a caixa de mensagem informando que os arquivos foram criptografados e tambem gera um arquivo com as instruções de recuperação.

<img width="384" height="274" alt="image" src="https://github.com/user-attachments/assets/21945fd8-1f1d-41cd-9dc8-8d848cd7b4c3" />

Com isso vemos que os nossos arquivos foram criptografados e não são mais legiveis como antes.

<img width="1478" height="356" alt="image" src="https://github.com/user-attachments/assets/6ee4276d-63be-4909-acf5-72439ee28341" />

    DESCRIPITANDO

Para o processo de decriptação vamos usar um script para reverter os efeitos do malware.

Vamos tentar carregar a chave e em caso positivo vamos fazer o processo de decriptação atravez da biblioteca Frenet que estamos usando.

<img width="1014" height="398" alt="image" src="https://github.com/user-attachments/assets/9b298b4f-8605-4875-a622-05fb5984a5d2" />

Para encontrar os arquivos e a nossa função principal será praticamente a mesma do processo de encriptação.

Ao final do processo recebemos a mensagem que tudo correu dentro do esperado e que os arquivos estão legiveis novamente.

<img width="415" height="206" alt="image" src="https://github.com/user-attachments/assets/6cb49485-3168-402e-a0dd-68616175c2ba" />
<img width="1460" height="387" alt="image" src="https://github.com/user-attachments/assets/5f063a50-3157-453b-8ee5-ac47c1d36a34" />


## 📚 Aprendizados
Durante o desenvolvimento deste projeto, alguns pontos importantes foram observados:
- **Criptografia é poderosa**: mesmo um código simples pode tornar arquivos inacessíveis.
- **Ambientes controlados são essenciais**: nunca execute esse tipo de código em sistemas reais.
- **Educação em cibersegurança**: entender como ataques funcionam ajuda a criar defesas mais eficazes.

---

## 🛡️ Como se Proteger
Para evitar ataques reais de ransomware:
- Mantenha **backups regulares** e em locais seguros.
- Utilize **antivírus e ferramentas de detecção de anomalias**.
- Evite abrir anexos ou links suspeitos em e-mails.
- Mantenha o sistema e softwares **sempre atualizados**.
- Promova a **conscientização em cibersegurança** dentro da organização.

---

## ✅ Conclusão
Este projeto é uma **simulação educacional** que mostra como ransomwares funcionam em sua essência.  
O conhecimento é a melhor defesa contra ataques reais.  
