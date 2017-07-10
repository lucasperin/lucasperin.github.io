Avaliacao 2
===========

## Descrição do trabalho
Em grupo, ou individualmente, criar uma ICP, emitir um certificado, cifrar e assinar um texto.

### Parte 1
Criar uma Infraestrutura de Chaves Públicas (ICP) com os seguintes requisitos:
* Uma Autoridade Certificadora (AC) **Raiz** (auto-assinada)
* Pelo menos uma AC **Intermediária** (requisição assinada pela AC raiz)
* Pelo menos uma AC **Final** (requisição assinada pela AC intermediária)

### Parte 2
Para cada membro do grupo, emitir um certificado assinado por uma **AC Final**

### Parte 3
Escrever um texto, cifrar em assinar
* Em um arquivo TXT, escreva o nome dos membros da equipe
* Cifre o arquivo txt utilizando ```openssl aes-128-cbc```
* Assinar o texto **cifrado** com o certificado de cada membro do grupo
  * Gere uma HASH utilizando **sha256** do arquivo cifrado
  * Para cada membro, assine o hash e guarde a assinatura em um arquivo

## Entregar
Zip com os documentos:
* Senha do AES-128-cbc
* Certificados de todas as ACs
* Certificado de todos os membros do grupo
* Texto cifrado
* Assinaturas

Entregar até dia 30/05


## Me ajuda!

Cifrar dado com AES: http://tombuntu.com/index.php/2007/12/12/simple-file-encryption-with-openssl/
Assinatura de dados (para assinar o txt cifrado): http://stackoverflow.com/questions/10782826/digital-signature-for-a-file-using-openssl
