#  FEITO POR Thaianna A. Hirota ;)  
   
# **REDE DE COMPUTADORES**   

---   
   
### **1- CONCEITO**   
Rede de computadores é o conjunto de dois ou mais computadores e dispositivos interconectados (impressoras, roteadores, switches, servidores, celulares, etc.), que conseguem trocar informações e compartilhar recursos entre si.   
   
**Vantagens de uma rede:**   
-> Compartilhar arquivos e dados;   
-> Compartilhar impressoras e outros recursos;   
-> Comunicação rápida, como: e-mails, mensagens internas, chamadas de voz e vídeo;   
-> Acesso ä Internet;   
-> Centralização de backups e segurança;   
   
---   
   
### **2- COMPONENTES PRINCIPAIS DE UMA REDE**   
**- Dispositivos finais:** computadores, notebooks, servicores, celulares, impressoras.   
**- Dispositivos de rede:** switch, roteador, firewall, ponto de acesso Wi-Fi.   
**- Meios de transmissão:** cabos (par trançado, fibra óptica) ou sinais sem fio (Wi-Fi, bluetooth, rádio).    
**- Protocolos de comunicação:** regras que permitem a comunicação, como o TCP/IP.   

---    
   
### **3- TIPOS DE REDE NA ESCALA GEOGRÁFICA**   
 **- LAN (local area network):** essa rede abrange uma área geográfica relativamente pequena, como dentro de uma casa, escola ou empresa.   
 **- MAN (metropolitan area network):** uma rede que cobre uma área geográfica maior, como uma cidade.   
 **- WAN (wide area network):** uma rede que abrange uma área ainda maior que  na MAN, abrangendo cidades, estados ou até mesmo países. No caso do Espírito Santo, seria uma rede que abrange a Grande Vitória.   
 **- WLAN:** rede local sem fio, o Wi-Fi.   

---   
   
### **4- TOPOLOGIA DE REDE FÍSICA**   
**- ESTRELA:** todos os dispositivos se conectam a um ponto central, como por exemplo, em um switch. Esse é o modelo mais utilizado.    
   
<img width="638" height="655" alt="image" src="https://github.com/user-attachments/assets/c2d4eae3-db90-4574-88b9-f6474cf40441" />   

       
**- ANEL:** os PC's ficam ligados em um ciclo fechado. Os dados circulam de um pra outro até chegarem ao destino. Um único PC fica com acesso diretamente ao modem, enquanto o PC 2, por exemplo, tem que passar pelo PC 1 pra ter acesso ä Internet, e assim sucessivamente. Para ficar sem dúvidas: O PC 1 recebe o acesso a Internet via modem/roteador. Quando o PC 2 quer acessar a Internet, ele envia os dados para o PC 1 (que é o que está próximo do anel, no caso, ele está diretamente conectado ao modem/roteador) e então, o PC 1 repassa o tráfego para o modem e devolve o resultado pelo anel. Se fosse o PC 3, ele passaria pelo PC 2, depois pelo PC 1 e faria todo o processo. O problema é que se o PC 1 cair, toda a rede fica sem internet. E é justamente por isso que não se usa mais essa topologia.   

<img width="593" height="653" alt="image" src="https://github.com/user-attachments/assets/4efa7912-ad58-4c55-bd66-3430700081a7" />   

No desenho acima, o PC 4, ele se conecta diretamente com o PC 1, então, ele pode enviar os dados pro 3, 2 e 1 ou diretamente para o PC 1.   

Existem outras topologias físicas, mas essas são as mais utilizadas. No caso, a estrela permanece no topo de utilização.   

---   

### **5- TOPOLOGIA DE REDE LÓGICA:**   
É a forma como os dados circulam dentro da rede, ou seja, como os computadores/dispositivos se comunicam. E isso inclui o caminho que a informação percorre e quais regras ou protocolos são usados.   
Não depende de como os cabos estão fisicamente ligados porque isso é topologia física.   
A topologia lógica se preocupa com o fluxo de informação e como o tráfego é controlado.   
Ex: imagine que você tem uma rede em topologia física estrela, onde todos estão ligado s a um switch. Fisicamente está na topologia física em estrela, mas logicamente, pode funcionar como um **broadcast** (em que todos recebem os dados, mas só o destino usa) ou até como **anel lógico** (se estiver configurada com protocolo tipo Token Ring).   
**5.1- Tipos de topologia lógica mais comuns:**   
**- Broadcast (Ethernet):** um PC envia os dados para todos, mas só o destinatário certo aceita. Essa é a lógica usada na maioria das redes LAN modernas.   
<img width="555" height="433" alt="image" src="https://github.com/user-attachments/assets/2dc095ce-62bb-4e49-8cd3-6af46e9a4b77" />   

Na imagem acima, o PC 1 pede informação para o servidor, que ao enviar a resposta, envia em modo broadcast (isso envia para todos os computadores), mas apenas o computador que pediu essa informação vai utilizar o dado. Os outros computadores irão descartar automaticamente essa informação.   
   


**- Anel lógico (Token Ring, FDDI):** onde um "token"circula de PC em PC, e só quem tem o token pode transmitir. Isso evita colisões de dados.    
Para essa topologia funcionar, cada computador que for ter esse compartilhamento de dados, precisa ter a placa de rede Token Ring (NIC própria) para poder participar do  anel lógico, e essa placa é incompatível com a Ethernet comum. Também deverá ter um cabo apropriado, geralmente é o cabo STP ou o UTP, e uma conexão MAU (multistation acess unit).   
Essa topologia caiu em desuso por conta de Ethernet, que é mais barata, atinge velocidades maiores e é mais fácil de gerenciar.
**- Ponto a ponto (Peer-to-peer):** é uma conexão direta entre dois dispositivos.    
Pode ser usado via cabo crossover Ethernet para ligar dois PCs diretamente ou por conexão Bluetooth.   
Porém ela só funciona bem entre dois dispositivos e não possui escalabilidade. A vantagem é que é simples de configurar, possui baixo custo porque não precisa de dispositivos de rede e é ideal para rede **muito** pequenas.      
**- Multiponto:** vários dispositivos compartilham o mesmo meio de comunicação (exemplo: barramento, Wi-Fi).   
Fácil de instalar, porém pode ter colisões de pacotes. Possui menor desempenho em redes grandes e se for feito apenas por meio físico e ele falhar, toda a rede para.   






### **6- COMO FUNCIONA**   
Basicamente é assim que funciona:   

1- Você contrata uma operadora de internet, seja ela, Claro, Vivo, Loga Internet, etc.   
2- Os cabos, geralmente de fibra óptica, são acrescentados do poste central para a sua casa.   
3- Colocam um modem roteador, já com wi-fi e várias entradas para conectar em vários dispositivos via cabo, que é conectado ao fio de fibra óptica que foi "puxado"do poste para a central de fios do seu prédio ou diretamente para o seu modem na sua residência.   
4- Ocorre a configuração do modem roteador.   
5- Por fim, o acréscimo e configuração do dispositivo que foi conectado a rede de internet da sua casa.   

<img width="444" height="429" alt="image" src="https://github.com/user-attachments/assets/f7c254ea-7392-4176-bcce-d58560a20faf" />


 

