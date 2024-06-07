# Global Solution
## Projeto Drone de Monitoramento de Condições Aquáticas
Este projeto consiste em um dispositivo IoT que capta dados de temperatura, salinidade, PH da água e umidade do ambiente e os disponibiliza para visualização em um site. O repositório contém o código do Arduino utilizado para capturar esses dados. 

## Protótipo Wokwi
[Clique aqui](https://wokwi.com/projects/399796899242490881) para ver o protótipo do projeto no wokwi. Como o simulador não tem os sensores de PH e salinidade, foi utilizado um potenciometro para simular a leitura desses sensores!


## Índice

- [Descrição do Projeto](#descrição-do-projeto)
- [Hardware Necessário](#hardware-necessário)
- [Instalação e Configuração](#instalação-e-configuração)
- [Funcionamento](#funcionamento)
- [Implementação](#implementação)

## Descrição do Projeto

O objetivo deste projeto é monitorar as condições da água em locais de difícil acesso e servir como objeto de interação para os turistas.

O dispositivo IoT é controlado por um controle e é responsável por coletar dados de temperatura, salinidade e ph e enviar essas informações para um servidor onde podem ser processadas por um especialista em dados, depois acessadas através de um site.

## Você também pode tantar montar o protótipo na sua casa!
### Hardware necessário

Para reproduzir este projeto, você vai precisar dos seguintes componentes:
- 1 Arduino Uno R3
- 1 Motor de Passos
- 3 resistores de 220 omns
- 3 Leds
- 1 Tela OLED modelo SSD1306
- 1 Módulo JoyStick
- 4 Push buttons
- 1 Potenciometro
- 1 Sensor dht11 ou dht22

### Instalação e configuração

1. Clone este repositório para o seu ambiente local:
    ```
    git clone https://github.com/victordz-dev/GlobalSolution_DroneDeMonitoramento
    ```

2. Abra o arquivo `droneDeMonitoramento.ino` na IDE do Arduino.

3. Instale as bibliotecas necessárias para o sensor, tela e motor:
- [DHT Sensor Library](https://downloads.arduino.cc/libraries/github.com/adafruit/DHT_sensor_library-1.4.6.zip)
- [Adafruit SSD1606](https://downloads.arduino.cc/libraries/github.com/adafruit/Adafruit_SSD1306-2.5.10.zip)
- [Adafruit GFX Library](https://downloads.arduino.cc/libraries/github.com/adafruit/Adafruit_GFX_Library-1.11.9.zip)
- [Stepper](https://downloads.arduino.cc/libraries/github.com/arduino-libraries/Stepper-1.1.3.zip?_gl=1*1023usy*_ga*MzQ2NTUyNTY1LjE3MTc1NDE2NDU.*_ga_NEXN8H46L5*MTcxNzc3OTA2NC4zLjAuMTcxNzc3OTA2OC4wLjAuMzM5NTQ1NjU1*_fplc*enI1VjJTSDB5JTJCd01qNDJWSWlxN3drOW5xTmZYVzdjNDlrNWlLRkxucWtGJTJGYTVvZXFLMXhhTmFYbjg2QkxRNGtSb1JKblhnQjRTaFBETFdWdnB2MXBhRG1nM09JMyUyRmdHYUl6bVYzeE5CRDNZbjRtMFptJTJGTEdRWU5BNyUyQnJnQSUzRCUzRA..)

4. Carregue o código no seu Arduino.

5. Após carregar o código no arduino, ele começará a captar as informações do `sensor` e `potenciometro`. Para observar esses dados, basta navegar pelo menu do display pelos `pushButtons`, utilizando:
- ⬆ e ⬇ para escolher a opção
- ➡ para entrar na opção escolhida
- ⬅ para voltar para o menu

6. Você também pode utilizar o `joyStick` para simular como seria o controle do drone, onde o eixo do motor aponta para a direção que as turbinas aquáticas se moveriam (ou seja, se você pressina para a esqueda, o eixo do motor se move para a direita, pois é para onde a turbina apontaria, fazendo assim o drone se mover para a esquerda).

## Funcionamento
Tente levar o dispositivo para diferentes lugares  e observe a oscilação dos dados captados pelo sensores pela tela.
Você pode também tentar aproximar o sensor DHT de alguns obetos, como um vaporizador ou até alguma coisa quente (tenha cuidado para não se machucar ou estragar algum sensor). Você também pode observar os valores de salinidade e ph se alterando quando altera a posição do `potenciometro` à vontade.

## Implementação

Visamos a implantação do sistema para coleta de dados das condições aquáticas em locais de difícil acesso, como lugares com muito lixo na superfície. Além disso, pretendemos utilizálos como ferramenta de aprendizado e consientização dos turístas, deixando-os navegar com o drone via controle remoto. Assim, conseguimos coletar os dados em tempo real dos oceanos, além de garantir a interatividade que é essencial para o aprendizado, tornando os passeios turísticos mais informativos.

## Construído com  🛠️  🛠️ 


![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&color=000)
