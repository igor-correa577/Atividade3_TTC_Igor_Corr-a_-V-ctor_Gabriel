#Descrição do sistema 

O sistema desenvolvido consiste em uma comunicação sem fio utilizando tecnologia LoRa entre dois dispositivos baseados no microcontrolador ESP32: um transmissor e um receptor. O transmissor é responsável por capturar mensagens digitadas pelo usuário via monitor serial e enviá-las através do módulo LoRa. Cada mensagem é numerada automaticamente, permitindo identificar a ordem de envio. O receptor, por sua vez, permanece em escuta contínua do canal de comunicação. Sempre que um pacote é recebido, ele realiza a leitura dos dados e exibe a mensagem no monitor serial, juntamente com o valor do RSSI (Received Signal Strength Indicator), que indica a intensidade do sinal recebido.

#Configuração

Hardwares utilizados:

- 2 ESP32
- 2 Módulos LoRa

Conexões ESP32 para LoRa:

-sinal SS - Pino 5 
-sinal Reset - Pino 14
-sinal DIO0 (interrupção) - Pino 2 

Comunicação realizada via interface SPI 
