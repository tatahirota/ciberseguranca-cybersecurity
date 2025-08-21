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

<p align="center">
<img width="638" height="655" alt="image" src="https://github.com/user-attachments/assets/c2d4eae3-db90-4574-88b9-f6474cf40441" /></p>   
   
       
**- ANEL:** os PC's ficam ligados em um ciclo fechado. Os dados circulam de um pra outro até chegarem ao destino. Um único PC fica com acesso diretamente ao modem, enquanto o PC 2, por exemplo, tem que passar pelo PC 1 pra ter acesso ä Internet, e assim sucessivamente. Para ficar sem dúvidas: O PC 1 recebe o acesso a Internet via modem/roteador. Quando o PC 2 quer acessar a Internet, ele envia os dados para o PC 1 (que é o que está próximo do anel, no caso, ele está diretamente conectado ao modem/roteador) e então, o PC 1 repassa o tráfego para o modem e devolve o resultado pelo anel. Se fosse o PC 3, ele passaria pelo PC 2, depois pelo PC 1 e faria todo o processo. O problema é que se o PC 1 cair, toda a rede fica sem internet. E é justamente por isso que não se usa mais essa topologia.   

<p align="center">
<img width="593" height="653" alt="image" src="https://github.com/user-attachments/assets/4efa7912-ad58-4c55-bd66-3430700081a7" /></p>      
   
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

<p align="center">
<img width="555" height="433" alt="image" src="https://github.com/user-attachments/assets/2dc095ce-62bb-4e49-8cd3-6af46e9a4b77" /></p>    

Na imagem acima, o PC 1 pede informação para o servidor, que ao enviar a resposta, envia em modo broadcast (isso envia para todos os computadores), mas apenas o computador que pediu essa informação vai utilizar o dado. Os outros computadores irão descartar automaticamente essa informação.   
   
   
**- Anel lógico (Token Ring, FDDI):** onde um "token"circula de PC em PC, e só quem tem o token pode transmitir. Isso evita colisões de dados.    
Para essa topologia funcionar, cada computador que for ter esse compartilhamento de dados, precisa ter a placa de rede Token Ring (NIC própria) para poder participar do  anel lógico, e essa placa é incompatível com a Ethernet comum. Também deverá ter um cabo apropriado, geralmente é o cabo STP ou o UTP, e uma conexão MAU (multistation acess unit).   
Essa topologia caiu em desuso por conta de Ethernet, que é mais barata, atinge velocidades maiores e é mais fácil de gerenciar.
**- Ponto a ponto (Peer-to-peer):** é uma conexão direta entre dois dispositivos.    
Pode ser usado via cabo crossover Ethernet para ligar dois PCs diretamente ou por conexão Bluetooth.   
Porém ela só funciona bem entre dois dispositivos e não possui escalabilidade. A vantagem é que é simples de configurar, possui baixo custo porque não precisa de dispositivos de rede e é ideal para rede **muito** pequenas.      
**- Multiponto:** vários dispositivos compartilham o mesmo meio de comunicação (exemplo: barramento, Wi-Fi).   
Fácil de instalar, porém pode ter colisões de pacotes. Possui menor desempenho em redes grandes e se for feito apenas por meio físico e ele falhar, toda a rede para.   
   
---   
   
### **6- COMO FUNCIONA**   
Basicamente é assim que funciona:   

1- Você contrata uma operadora de internet, seja ela, Claro, Vivo, Loga Internet, etc.   
2- Os cabos, geralmente de fibra óptica, são acrescentados do poste central para a sua casa.   
3- Colocam um modem roteador, já com wi-fi e várias entradas para conectar em vários dispositivos via cabo, que é conectado ao fio de fibra óptica, "puxado"do poste, para a central de fios do seu prédio ou diretamente para o seu modem na sua residência.   
4- Ocorre a configuração do modem roteador.   
5- Por fim, o acréscimo e configuração do dispositivo que foi conectado a rede de internet da sua casa.   

<p align="center">   
<img width="444" height="429" alt="image" src="https://github.com/user-attachments/assets/f7c254ea-7392-4176-bcce-d58560a20faf" /> </p>   
    
   
### **7- MODELOS DE REFERÊNCIA PARA REDE DE COMPUTADORES**   
Os modelos servem para padronizar a comunicação entre sistemas, ajudar a entender como os dados trafegam em uam rede e separar responsabilidades em camadas.    
**São dois tipos de modelos utilizados:** o modelo OSI e o TCP/IP. Irei explicar brevemente os dois modelos.   
**MODELO OSI:** é uma estrutura teórica desenvolvida pela ISO, que serve para padronizar e entender como os dados trafegam em uma rede. Esse processo é dividido em 7 camadas, e são elas:   
**7.1- Camada Física:** sua função principal é transmitir bits "crus"(0 e 1) pelo  meio físico, ou seja, cabos, rádio, luz, etc.   
Nessa camada, ocorre a conversão de dados em sinais físicos (elétricos, ópticos, radiofrequência, etc.), também define os meios de transmissões (cabos UTP, fibra óptica, Wi-Fi, Bluetooth) e trabalha com bitrate, voltagem, modulação e frequência.   Exemplos:   
Meios físicos: RJ-45, Wi-Fi, fibra.   
Padrões: IEEE 802.11 (Wi-Fi), 802.3 (Ethernet), DSL, USB.   
- **Problemas possíveis:** cabos danificados, conectores frouxos, porta física quebrada, interferência eletromagnética (EMI), mal terminação de cabo, falha de energia, falha em NICs ou switches, má configuração duplex/velocidade, sinal fraco (Wi-Fi).
   
- **Ferramentas para diagnóstico:** testador de cabo, multímetro, wireshark (detecta falhas de transmissão, LED na placa de rede (indica conexão física).   
Quanto a luzes de link nos equipamentos: são leds geralmente encontrados em switches, roteadores, nics (placas de rede) e modem. Como analisar: se a cor estiver verde e fixo, a conexão está boa e ativa, caso esteja verde piscando, o tráfego de dados está fluindo. Se estiver amarelo/vermelho/desligado pode ser problema na conexão ou no cabo. Se o led estiver apagado pode-se ter: cabo danificado, NIC desativada, porta errada, switch desligado, problema na alimentação.   
O testador de cabos é um dispositivo que verifica continuidade, pares trocados, abertos ou curtos em cabos de rede. Como usar: conecte uma ponta do cabo no transmissor e outra no receptor (remoto), daí ligar o testador e observar os leds (geralmente enumerados de 1 a 8+ G). A sequência correta que irá acender é 1-2-3-4-5-6-7-8, significa que o cabo está OK. Caso a sequência esteja trocada ou pinos não acendendo, os pares estão trocados ou rompidos então temos de refazer a ponta do cabo. E se dois leds acenderem ao mesmo tempo ou todos estiverem piscando irregularmente é porque está em curto. Aqui também devemos refazer o conector dos cabos. Se não funcionar em nenhum dos casos, devemos trocar o cabo inteiro. Se também não funcionar, o problema está na camada 2 do modelo OSI.

   Foto do testador de cabos:
  <p align="center">
  <img width="333" height="270" alt="image" src="https://github.com/user-attachments/assets/ecdf9f61-c4af-4044-b79c-0459ff4c6a5e" /> </p>   

Multimetro serve para testar a continuidade elétrica dos cabos. Como usar: coloque na funcão continuidade (símbolo de som ou diodo), a ponta preta vai na tomada "COM"e a vermelha no slot marcado para tensão/resistência/continuidade. Então, para testar, encoste as pontas nos dois lados (extremidades) de um mesmo fio do cabo RJ-45, se apitar, o fio está contínuo, se não apitar, o fio está rompido.    

   Foto do multímetro:   
 <p align="center">
 <img width="500" height="333" alt="image" src="https://github.com/user-attachments/assets/3d746d1a-bff9-4973-b659-7706708609ad" /></p>   
   
   
OTDR é uma ferramenta usada para fibra óptica e ela mede perdas, falhas, quebras e distância até o problema. Ela envia pulsos de luz pela fibra e mede o tempo de retorno (eco/reflexão) para detectar os conectores defeituosos, emendas ruins e até quebras na fibra. Geralmente é utilizada para verificar a integridade de links de fibra, principalmente em longas distâncias, superiores a 100m.     

   Foto do OTDR:   
   <p align="center">
   <img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/66712eca-c245-45a1-98f9-9100af72e157" /></p>      
   
Loopback Plugs é um conector especial que reflete o sinal de volta para o equipamento. Como usar: conecta ele na porta de rede (NIC, switch) e se a luz de link acender ou testes passarem, a porta está funcionando. Se não acender, o problema pode ser na porta.   
Monitorar estatísticas de interface (erros e colisões): devemos usar comandos ou ferramentas de monitoramento na máquina ou no switch. Em Windows (cmd), utilizamos: netstat -e, em Linux: ipconfig eth0.
No Windows, o netstat -e vai exibir estatísticas de pacotes enviados, recebidos, erros e colisões. Números altos nos campos de erro indicam problemas físicos.
No Linux, o ifconfig vai ter uma saida tipo: RX packets:696011 errors:0 dropped:0 overruns:0 frame:0   
TX packets:524673 errors:0 dropped:0 overruns:0 carrier:13 collisions:0
- Normalidade: erros, dropped, frame, collisions, devem estar em zero ou próximo. carrier pode aparecer em alguns caso.
- Anormalidade: erros indica CRC, frames fora de padrão ou incompatibilidade de duplex/velocidade. frame pode ser frames malformados (CRC inválido ou tamanho incoerente), dropped, overruns podem ser pacotes não processados por falta de buffer ou CPU ocupada. collisions pode ser excessivas colisões indicando problema de duplex ou congestão, e valores normais são muito baixos, exemplo, <00,1%/.
 
- No Linux, utilizando o ethool -S <interface>, mostra estatísticas detalhadas como: rx_errors, rx_crc_errors, rx_frame_errors, rx_over_errors, etc. Zeros indicam tudo bem, qualquer valor que não seja zero, aponta para testes de cabos, mudanças de porta, ajustes de duplex/velocidade ou substituição de hardware.
-  **rx_erros** são pacotes recebidos com erros de checksum sendo sinal de cabo ruim, interferência ou duplex incorreto. frame são pacotes com quadros corruptos e indica problemas físicos ou malterminações.
  **rx_drp** são pacotes recebidos descartados por buffer cheio, pode ser saturação ou desempenho do sistema, em que há fila de recepção cheia, Kernel/driver não conseguiu lidar com a entrada, problemas físicos (em menor escala) e/ou congestionamento geral. Para resolver"atualizar os drivers, evitar broadcast/multicast em excesso na rede, verificar topologia de rede (muitas máquinas em um único switch pode gerar flooding) e monitorar com as ferramentas iftop, nload, netdata.
  **rx_ovr** são pacotes perdidos por sobrecarga do kernal com CPU ou interrupções lentas em o sistema não conseguiu processar os pacotes recebidos rápido o suficiente e eles foram descartados por falta de buffer. Isso não é necessariamente um problema físico, mas muitas vezes está relacionado a alta carga de rede, problemas no driver da placa, hardware fraco ou mal dimensionado e/ou buffer de recepção muito pequeno. Para resolver, vamos seguir o passo a passo: atualizar os drivers da placa de rede, verificar o uso de CPU/RAM, reduzir o tráfego ou isolar rede pesadas (VLANS, QoS), se possível, utilizar placa de rede com mais buffer ou offload (tipo a da intel com suporte a TCP offloading), em switches gerenciáveis devemos aumentar o buffer por porta (cuidado que nem todos os switches permmitem isso) e também verificar as interrupções da NIC.
  **framme** é um problema puramente físico em que o quadro Ethernet foi recebido com tamanho inválido, erro de alinhamento ou erro de CRC e pode ser causado por cabo de rede com defeito, cabo de qualidade ruim ou mal crimpado, conectores soltos ou oxidados, EMI (cabos passando perto de motores, lâmpadas, etc.), má terminação (em fibra ou cabos longos). Para resolver, devemos testar e trocar os cabos de rede, recrimpar os conectores, evitar passar cabo junto com cabos de energia ou motores e verificar o  padrão de crimpagem, se é A ou B.
  **collisions** são colisões que acontecem quando dois dispositivos tentam transmitir ao mesmo tempo na mesma rede Ethernet e é comum em hubs antigos e principalmente, em duplex se está desajustado e valor muito acima de zero é ruim. Nos switches modernos, só acontece se houver desajuste de duplex como por exemplo, se um lado está Full Duplex e o outro está Half Duplex. Para resolver, temos que verificar as configurações de duplex/velocidade em ambos os lados (computador e switch). O ideal é utilizar auto-negociação em ambos e se precisar definir manualmente, configurar full duplex nos dois lados. obs: as velocidados em ambos também devem coincidir.   

   
- **Como resolver:** substituir cabos/conectores, ajustar configurações de duplex/velocidade, garantir alimentação estável, substituir hardware defeituoso.
   
Para troca do RJ-45, temos as duas formas de sequência de padrões mais utilizados:   
   
<p align="center">
<img width="623" height="415" alt="image" src="https://github.com/user-attachments/assets/e502bee1-b2db-4fb3-aedf-513432fd4c04" /></p>    
   




