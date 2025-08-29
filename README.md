



# Guia: Utilizando o Sensor DHT22 com ESP32

## 1. Montagem do Circuito

Coloque a **placa ESP32** na **protoboard**:

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/WhatsApp%20Image%202025-08-27%20at%2013.58.46.jpeg" width="400"/>

Depois, conecte os cabos nos seguintes pontos:

* **Fio preto** → **GND**
* **Fio vermelho** → **5V/VIN**
* **Fio laranja** → **Pino Digital**

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/WhatsApp%20Image%202025-08-27%20at%2013.37.24.jpeg" width="400"/>

---

## 2. Instalação da Biblioteca `Bonezegei_DHT11`

Essa biblioteca é necessária, pois contém as funções que vamos utilizar no programa.

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/Captura%20de%20tela%202025-08-27%20142821.png" width="400"/>

---

## 3. Código de Funcionamento 🧑‍💻

Escreva o código abaixo para que o **DHT22** funcione corretamente:

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/WhatsApp%20Image%202025-08-27%20at%2013.37.10.jpeg" width="400"/>

### Como o Código Funciona:

* Primeiro, inclua a biblioteca com `#include`
* Defina o **pino digital** utilizado pelo sensor
* No `setup()`, inicialize a comunicação serial e o sensor com `dht.begin();`
* No `loop()`:

  * Os valores de temperatura (`tempDeg`) e umidade (`hum`) são lidos
  * As informações são exibidas no **monitor serial**

---

## 4. Conexão com o Computador

O cabo usado foi do tipo **Micro USB**.

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/WhatsApp%20Image%202025-08-27%20at%2013.58.14.jpeg" width="400"/>

---

🔎 Observação: A foto mostra apenas a ligação via cabo USB, sem outros componentes conectados.

---

## 4.1 Enviando o Código para o ESP32

Na **IDE Arduino**, clique no botão de **upload (seta para a direita no canto superior esquerdo)** para gravar o programa na placa.

<img src="https://github.com/GustavoLoghan/Sensor_DHT22/blob/main/2/Captura%20de%20tela%202025-08-27%20143351.png" width="400"/>

---

## 4.5 Se aparecer o erro "BOOT"

Em alguns modelos, pode ser preciso:

1. Pressionar o botão **BOOT** durante o envio do código
2. Soltar o botão logo após o início da gravação

---

## 5. Finalização 🎉

Seguindo todos os passos, seu projeto deve estar funcionando sem problemas! 😁👍



