<h1 align="center"> Sprint 4 - Sensor de Força + LCD + LED no ESP32 | Challenge IBM </h1> <br>
<p align="center">
  <a href="https://github.com/punk272/checkpoint5_edge">
    <img alt="Circuito" title="Wokwi" src="https://imgur.com/rHbCDoS.png" width="1000">
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

Para o funcionamento do nosso projeto de criação e cheacagem de saúde de um de um servidor usamos uma máquina virtual atráves da plataforma VMware e então usamos o Ubunto para baixar o sistema operaciaonal Linux, após isso fizemos a instalação da imagem na máquina virual e configuramos a rede de VM como bridge. Após a instalação da imagem na máquina virtual baixamos o postman e suas collection necessárias para fazer a intalação do Docker e por fim entramos na máquina virtual e através do terminal fizemos usamos alguns comandos para instalar o docker gerando uma plataforma backend para o nosso servidor para obter dados importantes da máquina virtual coomo IP, e por fim usamos esses dados para executar a ação de health check e concluir nosso trabalho.






## Componentes

Peças usadas na construção deste circuito:

* 1 x Placa ESP32
* 1 x Breadboard
* 1 x Sensor DHT11 ou DHT22
* 1 x Resistor Dependente da Luz (LDR)
* 1 x Resistor de 10k Ohms
* 8 x Jumpercables

## Requisitos

* Collection FIWARE Postman (FIWARE.postman_collection.json): Recebe e armazena dos dados do ESP32.
* Biblioteca Paho-MQTT (FIAP_Fiware_Paho.ipynb): Leitura dos dados obtidos pelo ESP32.
* Código Fonte IDE Arduino (fiware_ngsi_mqtt_esp32.ino): Código principal do circuito, faz todo o processo de captura, leitura de dados e comunicação do microcontrolador com o servidor IoT através de Wi-Fi.
* Gráfico de Luminosidade (sth-comet.py): Obtém os dados de luminosidade para a criação de um gráfico em função do tempo.
* Docker e Docker-Compose Ubuntu Server LTS (docker-compose.yml): Software onde o servidor será instalado (Clique <a href=https://docs.docker.com/engine/install/ubuntu/> aqui </a> para ver as instruções de instalação.

## Autores

- **Leonardo Mansur**
- **Luís Guilherme**
