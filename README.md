<h1 align="center"> Sprint 4 - Sensor de Força + LCD + LED no ESP32 | Challenge IBM </h1> <br>
<p align="center">
  <a href="https://github.com/punk272/sprint4_grupo7_EDGE">
    <img alt="Circuito" title="ESP32HX711" src="https://i0.wp.com/randomnerdtutorials.com/wp-content/uploads/2022/03/ESP32-load-cell-HX711-amplifier.jpg?resize=1024%2C576&quality=100&strip=all&ssl=1" width="1000">
  </a>
</p>


## Tópicos do projeto

- [IoT](#iot)
- [Projeto](#projeto)
- [Componentes](#componentes)
- [Requisitos](#requisitos)
- [Autores](#autores)

## IoT

A Internet das Coisas (IoT, na sigla em inglês) é uma revolução tecnológica que tem transformado a maneira como interagimos com o mundo à nossa volta. Ela se refere à interconexão de dispositivos, objetos e sistemas por meio da internet, permitindo que eles coletem, compartilhem e analisem dados de forma automatizada. Neste texto, exploraremos os conceitos envolvidos na IoT e a importância dessa tecnologia.

<img src="https://blog.pix.com.br/wp-content/uploads/2020/04/original-9f74f5d4901a799779f531c1e84426ac.jpg">

<h2>Conceitos IoT:</h2>
Dispositivos Conectados: A base da IoT são os dispositivos, que podem ser qualquer coisa, desde sensores e smartphones até eletrodomésticos e veículos, que são equipados com capacidade de comunicação e sensores para coletar informações.

Conectividade: Esses dispositivos se comunicam através da internet ou outras redes de comunicação sem fio, como Bluetooth e RFID. A conectividade é essencial para que os dados sejam transmitidos e processados em tempo real.

Sensores e Atuadores: Sensores são responsáveis por coletar informações do ambiente, como temperatura, umidade, pressão, localização, entre outros. Atuadores são dispositivos que realizam ações com base nas informações coletadas, como ligar ou desligar um aparelho.

Processamento de Dados: Os dados coletados pelos dispositivos são enviados para servidores, onde são processados, analisados e armazenados. Algoritmos de análise de dados são frequentemente usados para extrair informações úteis a partir dos dados brutos.

Aplicativos e Interfaces: A IoT cria a necessidade de aplicativos e interfaces que permitam aos usuários controlar, monitorar e interagir com os dispositivos de forma intuitiva. Isso pode ser feito através de aplicativos móveis ou interfaces web.

<h2>A Importância da Internet das Coisas:</h2>
Eficiência Operacional: A IoT tem o potencial de otimizar operações em diversas áreas, como agricultura, indústria, saúde e logística. Ela permite o monitoramento em tempo real de máquinas, equipamentos e processos, tornando-os mais eficientes e econômicos.

Melhoria na Qualidade de Vida: Na área da saúde, dispositivos médicos conectados podem monitorar pacientes remotamente, permitindo tratamentos mais personalizados e reduzindo custos hospitalares. Em casa, dispositivos inteligentes tornam a vida mais conveniente e segura.

Sustentabilidade Ambiental: A IoT pode ser usada para monitorar e controlar o consumo de recursos naturais, como energia e água, contribuindo para a redução do desperdício e a conservação do meio ambiente.

Segurança e Monitoramento: A IoT também desempenha um papel crucial na segurança, permitindo a vigilância e monitoramento de áreas remotas e o acompanhamento em tempo real de sistemas de segurança.

Novos Modelos de Negócios: A IoT está criando oportunidades para novos modelos de negócios, como serviços baseados em assinatura e produtos conectados. Empresas podem oferecer serviços adicionais, como análise de dados e manutenção preventiva.

Desenvolvimento da Inteligência Artificial: A IoT gera grandes volumes de dados, que são alimentados em algoritmos de aprendizado de máquina e inteligência artificial. Isso impulsiona o desenvolvimento dessas tecnologias, tornando-as mais inteligentes e eficazes.

## Projeto

Nosso projeto consiste em um circuito ESP32 com um Sensor de Força implementados em uma lixeira para calcular o seu peso e indicar se a lixeira está vazia/com pouco peso, com peso médio ou muito pesada utilizando um display LCD e três LEDs.
Além disso, capturar os dados de peso e, utilizando MQTT, armazenar esses valores em uma plataforma back-end para facilitar a manutenção das lixeiras, tudo isso em tempo real.

## Componentes

Peças usadas na construção deste circuito:

* 1 x Placa ESP32
* 1 x Breadboard
* 1 x Sensor de Força HX711
* 3 x Resistores de 10k Ohms
* 1 x Resistor de 4.7k Ohms
* 8 x Jumpercables

## Requisitos

* Collection FIWARE Postman (FIWARE.postman_collection.json): Recebe e armazena dos dados do ESP32.
* Biblioteca Paho-MQTT (FIAP_Fiware_Paho.ipynb): Leitura dos dados obtidos pelo ESP32.
* Código Fonte IDE Arduino (codigo_sprint4.ino): Código principal do circuito, faz todo o processo de captura, leitura de dados e comunicação do microcontrolador com o servidor IoT através de Wi-Fi.
* Docker e Docker-Compose Ubuntu Server LTS (docker-compose.yml): Software onde o servidor será instalado (Clique <a href=https://docs.docker.com/engine/install/ubuntu/> aqui </a> para ver as instruções de instalação.

## Autores

- **Leonardo Mansur - RM:551659**
- **Luís Guilherme - RM:98688**
- **Arthur Abreu - RM:98283**
- **Carlos Roberto - RM:551877**
