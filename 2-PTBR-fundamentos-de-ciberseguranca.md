# **FUNDAMENTOS DE CIBERSEGURANÇA**    

<br>  

## **O QUE É CIBERSEGURANÇA?**   
Basicamente é a prática de proteger dispositivos, redes e dados contra ataques, roubo ou danos referentes aos ativos citados anteriormente.  
O objetivo é garantir que as informações permaneçam seguras e protegidas contra ameaças, como hacker e vírus.  
<br>  
______________________________________________________________________________________________________________________________________________
## OS TRÊS PILARES FUNDAMENTAIS PARA CONSEGUIR APLICAR A CIBERSEGURANÇA NO DIA A DIA:    
São conhecidos como CID.   
**C**= Confidencialidade, pois temos que garantir que a informação seja acessada apenas por pessoas ou sistemas autorizados.  
**I**= Integridade, devemos assegurar que os dados não sejam alterados de forma não autorizada, seja por erro ou ataque.   
**D**= Disponibilidade, aqui, garantimos que os dados e sistemas estejam acessíveis e funcionando quando necessário, não importa a situação.   
<br>   
_______________________________________________________________________________________________________________________________________________
## CONFIDENCIALIDADE NA PRÁTICA:

**CRIPTOGRAFIA DE DADOS**: utilização de criptografia para proteger informações sensíveis (senhas ou dados financeiros, podendo ser em trânsito, e-mails ou rede, ou em repouso, armazenados em disco).   
   
**Aplicação 1**: Criptografia em trânsito. Configurar e garantir que todos os dados críticos cpritografados usem protocolos como TLS/SSL (transport layer security / secure sockets layer) para comunicação e criptografia de disco, protegendo entre servidores e clientes, como em sites HTTPS e e-mails.   
    Exemplo:  
    Passo 1: a empresa/analista deve adquirir ou gerar um certificado SSL/TLS para o servidor que será usado para criptografar os dados em trânsito. Para sites: pode utilizar ferramentas como o "Let's Encrypt" para obter certificados gratuitos. Para servidores de e-mail (SMTP/IMAP/POP3): deve configurar o servidor de e-mail para suportar o TLS.   
    UTILIZANDO O LET'S ENCRYPT:
    
