# 1. Introdução

O projeto tem como objetivo monitorar a temperatura e umidade do ambiente utilizando o sensor DHT11 conectado ao microcontrolador ESP32.
Além disso, dois LEDs foram adicionados para indicar visualmente a condição da temperatura:

🔴 LED vermelho → ambiente quente (acima de 25 °C)

🔵 LED azul → ambiente frio ou normal (até 25 °C)

2. Materiais Utilizados
<div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <img src="https://github.com/user-attachments/assets/dbb5adae-6f1e-4d86-93a2-04bc007998db" style="width:80px; height:auto;" /> <span>1x ESP32 DevKit</span> </div> <div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <span>1x Sensor DHT11</span> </div> <div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <img src="https://github.com/user-attachments/assets/ed78b9e0-6ba4-4abc-8431-8ec26bd54b72" style="width:70px; height:auto;" /> <img src="https://github.com/user-attachments/assets/0d623fb3-924b-4d26-87cc-8b7f36f56e56" style="width:70px; height:auto;" /> <span>1x LED vermelho + resistor 220 Ω</span> </div> <div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <img src="https://github.com/user-attachments/assets/6225fe3d-b99f-4420-bfd9-1dca9182048b" style="width:70px; height:auto;" /> <img src="https://github.com/user-attachments/assets/0d623fb3-924b-4d26-87cc-8b7f36f56e56" style="width:70px; height:auto;" /> <span>1x LED azul + resistor 220 Ω</span> </div> <div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <img src="https://github.com/user-attachments/assets/d156e551-28df-4287-97f1-e562f089a54b" style="width:80px; height:auto;" /> <span>Jumpers (fios de conexão)</span> </div> <div style="display:flex; align-items:center; gap:12px; margin-bottom:12px;"> <img src="https://github.com/user-attachments/assets/2f37cbf6-e85e-4b8f-aee8-b299d4615fa0" style="width:100px; height:auto;" /> <span>Protoboard</span> </div>



# 3. Montagem do Circuito
Conexão do Sensor DHT11

Sinal (DATA) → GPIO 21 do ESP32

VCC → 3.3V do ESP32

GND → GND do ESP32

Conexão dos LEDs

LED vermelho (com resistor) → GPIO 18

LED azul (com resistor) → GPIO 19

Outro terminal dos resistores → GND do ESP32

# 4. Passo a Passo da Montagem

Etapa 1 – Inserindo o ESP32 na Protoboard

O ESP32 foi posicionado no centro da protoboard para facilitar as conexões.

<img src="https://github.com/user-attachments/assets/42942e24-8371-4f97-93e4-b2758e76d679" style="width:220px; height:auto; margin-bottom:12px;" />

Etapa 2 – Inserindo os LEDs

Foram adicionados o LED vermelho e o LED azul, respeitando a polaridade:

Terminal maior (ânodo) ligado ao pino do ESP32

Terminal menor (cátodo) conectado ao GND via resistor de 220 Ω

<img src="https://github.com/user-attachments/assets/d3c5de8a-9188-479c-a1d9-8d3b72edae8c" style="width:220px; height:auto; margin-bottom:12px;" />

Etapa 3 – Conexão dos Resistores

Os resistores foram ligados em série com cada LED para proteger os LEDs de sobrecarga.

<img src="https://github.com/user-attachments/assets/812b5c2a-a1ae-44ca-9c16-6e790405e971" style="width:220px; height:auto; margin-bottom:12px;" />

Etapa 4 – Conectando o Sensor DHT11

O sensor DHT11 foi colocado na protoboard e conectado aos pinos do ESP32.

<img src="https://github.com/user-attachments/assets/2996b890-ff86-427d-a01a-4c141b97a2c5" style="width:220px; height:auto; margin-bottom:12px;" />

Etapa 5 – Ligações Finais com Jumpers naty naty sonsa

Jumpers foram usados para conectar o ESP32 aos LEDs e ao DHT11.

<img src="https://github.com/user-attachments/assets/ae7f4973-40ee-4a2f-aa8e-0a61e2ee44ef" style="width:220px; height:auto; margin-bottom:12px;" />

Etapa 6 – Teste do Circuito

Após subir o código para o ESP32:

LED vermelho aceso → temperatura > 25 °C

LED azul aceso → temperatura ≤ 25 °C

Exemplo de funcionamento:

<div style="display:flex; gap:12px;"> <img src="https://github.com/user-attachments/assets/6d0fa6fc-d808-4e0f-99d7-537ccde41cde" style="width:220px; height:auto;" /> <img src="https://github.com/user-attachments/assets/fc2f91cd-ef5b-412e-8ba5-8f4207f8a5b0" style="width:220px; height:auto;" /> </div>
