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
_____________________________________________________________________________________________________________________________   
   
## CONFIDENCIALIDADE NA PRÁTICA:   

**1- IDENTIFICAR OS DADOS SENSÍVEIS;**   
**2- CLASSIFICAR OS DADOS SENSÍVEIS;**   
**3- IMPLEMENTAR CONTROLES DE ACESSO;**   
**4- CRIPTOGRAFAR DADOS;**   
**5- PROTEGER DADOS EM USO;**  
**6- MONITORAR E AUDITAR;**   
**7- TREINAR FUNCIONÁRIOS;**  
**8- IMPLEMENTAR POLÍTICAS DE SEGURANÇA;**   
**9- PROTEGER DISPOSITIVOS DE REDE;**   
**10- TESTAR E MELHORAR;**   

**1- IDENTIFICAR DADOS SENSÍVEIS:** são dados pessoais (nome, endereço, CPF, e-mail, etc), dados financeiros (número de cartáo de crédito, transações bancárias,etc), dados de login (senha, token de autenticação, etc), histórico de compras (produtos adquiridos, preferências de consumo, etc), histórico médico, etc.   
   Para realizar um mapeamento de todos os dados que precisam de proteção, deve-se fazer isso de forma eficiente, e pode utilizar as ferramentas de **Data Center** ou **Data Classification**, pois ajudam a localizar e classificar os dados sensíveis em sistemas, rede e armazenamentos. Uma ferramenta gratuita para Windows e Debian é o **Apache Tika** (arquivos locais), com plugins de segurança, ou alternativamente, o **OpenDLP** (para banco de dados), **SpiderFoot**, **Veracript**, entre outras ferramentas.   
   TÓPICO DETALHADO SOBRE DATA DISCOVERY E DATA CLASSIFICATION: [EM CONSTRUÇÃO]   
   TÓPICO DETALHADO SOBRE APACHE TIKA: [ EM CONSTRUÇÃO]   
   TÓPICO SOBRE OPENDLP: [EM CONSTRUÇÃO]   
   TÓPICO SOBRE SIPERFOOT: [EM CONSTRUÇÃO]   
   TÓPICO SOBRE VERACRIPT: [EM CONSTRUÇÃO]   


   **2- CLASSIFICAR OS DADOS:** classificar de acordo com o nível de sensibilidade, público (nome de produto, avaliação de cliente), interno (histórico de compras), confidencial (CPF, endereço de e-mail), altamente confidencial (número de cartáo de crédito, senha). Nessa fase, o objetivo é implementar ferramentas e processos para aplicar a classificação definida anteriormente utilizando ferramentas que ajudam a identificar, rotular e proteger os dados com base em sua sensibilidade.


   

**CRIPTOGRAFIA DE DADOS**: utilização de criptografia para proteger informações sensíveis (senhas ou dados financeiros, podendo ser em trânsito, e-mails ou rede, ou em repouso, armazenados em disco).   
   
**Aplicação 1**: Criptografia em trânsito. Configurar e garantir que todos os dados críticos cpritografados usem protocolos como TLS/SSL (transport layer security / secure sockets layer) para comunicação e criptografia de disco, protegendo entre servidores e clientes, como em sites HTTPS e e-mails.   
    Exemplo:  
    Passo 1: a empresa/analista deve adquirir ou gerar um certificado SSL/TLS para o servidor que será usado para criptografar os dados em trânsito. Para sites: pode utilizar ferramentas como o "Let's Encrypt" para obter certificados gratuitos. Para servidores de e-mail (SMTP/IMAP/POP3): deve configurar o servidor de e-mail para suportar o TLS.   
    UTILIZANDO O LET'S ENCRYPT:
    
