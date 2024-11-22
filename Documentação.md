Ana Paula Nascimento Silva  RM552513  2TDSR

Calina Thalya Santana Da Silva RM552523 2TDSR

Anna Beatriz Soares Camargo  RM99814 2TDSA

Marcelo Henrique  Borgas  RM98893 2TDSA

Michael Bombo Leon RM551382 2TDSA

![image](https://github.com/user-attachments/assets/9b24d273-a3ec-4440-b072-1259492b40cc)



Projeto IoT: Controle de Luz com Movimento e Luminosidade


Somos a Hydrio Mind, e nosso objetivo principal é desenvolver soluções inteligentes que promovam a economia de recursos,
como água e energia, através da tecnologia. Este projeto é um exemplo prático de nossa missão,
focado na economia de energia ao automatizar o controle de iluminação com base nas condições do ambiente.

A proposta é simples, mas eficaz: usar sensores de movimento e luminosidade para acender a luz apenas quando necessário,
de forma pesonalizada pelo usuario, reduzindo o consumo desnecessário de energia elétrica. Nossa solução se comunica com a
internet via MQTT, permitindo que dados sejam monitorados e configurações ajustadas remotamente.

Este projeto foi realizado no Wokwi. Este é o link do projeto feito no wokwi:
https://wokwi.com/projects/415203281283016705



Hardware Utilizado:

-ESP32

-Sensor de Movimento PIR

-Sensor de Luminosidade (fotoresistor)

-LED

-Resistores

Tecnologias:

-Protocolo MQTT

-Broker público: test.mosquitto.org


Principais Funcionalidades:

Detectar movimento e luminosidade.

Controlar o LED com base nas condições do ambiente.

Publicar informações no MQTT: luminosidade, estado da luz, configurações atuais e informações coletadas pelos sensores.

Receber configurações remotas via MQTT, como o limiar de luz e o tempo que a luz deve permanecer acesa, assim o sensor pode ter as configurações desejadas pelo usuario.

![image](https://github.com/user-attachments/assets/270e2bf7-dfc7-401d-996c-b5c239c7199b)

![image](https://github.com/user-attachments/assets/a90696e8-77fb-48d0-84ae-de90d5f1aa5b)

Na Dashboard do Node-RED desenvolvida para este projeto, foram implementadas funcionalidades que permitem monitorar e controlar diversos aspectos do sistema em tempo real. A interface foi projetada para ser intuitiva e interativa, com as seguintes características principais:

Controlador de Sensor de Luz:

Exibe o status atual do sistema, como "Pouca luz natural, porém sem movimento", atualizado com base nos sensores e na lógica do código.
Mostra o nível de iluminação atual captado pelo sensor de luminosidade, permitindo o acompanhamento da intensidade da luz no ambiente.
Luz Natural Máxima (Controlável):

Permite ajustar o limiar de luminosidade máxima diretamente pela Dashboard. Esse valor determina a intensidade de luz ambiente necessária para que o sistema decida se a luz deve ser acesa ou não.
O ajuste facilita a personalização do sistema para diferentes condições de luminosidade em cada ambiente.
Nível da Luz:

Um indicador gráfico que varia de 0 a 4100, representando em tempo real a intensidade da luz ambiente captada pelo sensor. Isso ajuda a visualizar o impacto da luz natural e artificial no ambiente.
Controlador de Tempo de Desligamento das Luzes:

Exibe o tempo atual em que a luz está ligada, ajudando no acompanhamento do sistema em funcionamento.
Oferece um controle ajustável para configurar o temporizador da luz em segundos, determinando por quanto tempo a luz deve permanecer acesa após ativada.
A Dashboard integra todas essas funcionalidades de maneira prática, reforçando o objetivo do projeto de combinar eficiência e usabilidade, ao mesmo tempo que promove a economia de energia através de ajustes simples e precisos.
![image](https://github.com/user-attachments/assets/e1cbd44e-6258-4026-88dc-5db880b45ef8)

Código-fonte do esp32: https://github.com/MikW02/HYDRIOMIND_GS/blob/main/CodigoFonteEsp32
