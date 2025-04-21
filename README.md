📘 Introdução

O Arduino constitui uma plataforma de prototipagem eletrônica de código aberto amplamente adotada em ambientes educacionais, científicos e industriais. Baseado em uma arquitetura de hardware e software acessível, o Arduino visa simplificar o desenvolvimento de sistemas embarcados, proporcionando uma interface intuitiva para a criação de dispositivos interativos.

![Arduino UNO](imagens/arduino_blink-fast.gif)

🎯 Objetivo

A principal finalidade do Arduino é viabilizar o desenvolvimento de projetos de automação e controle, promovendo a integração entre sensores, atuadores e sistemas computacionais. A plataforma permite a experimentação prática de conceitos de eletrônica e programação, sendo amplamente utilizada em pesquisas acadêmicas, projetos de extensão e desenvolvimento de soluções voltadas à Internet das Coisas (IoT), robótica e educação tecnológica.

✅ Conclusão

Dada sua flexibilidade, baixo custo e extensa comunidade de suporte, o Arduino representa uma ferramenta pedagógica e tecnológica de grande relevância. Seu uso contribui significativamente para a formação técnica e científica de estudantes e profissionais, além de impulsionar a inovação em diversas áreas do conhecimento.

# Codigo semanaforo

// Definição dos pinos

const int ledVerde = 2;

const int ledVermelho = 3;

const int ledAzul = 4;

void setup() {

  pinMode(ledVerde, OUTPUT);
  
  pinMode(ledVermelho, OUTPUT);
  
  pinMode(ledAzul, OUTPUT);
  
}

void loop() {

  // Sinal verde 
  
  digitalWrite(ledVerde, HIGH);
  
  digitalWrite(ledAzul, LOW);
  
  digitalWrite(ledVermelho, LOW);
  
  delay(5000); // 5 segundos

  // Sinal amarelo 
  
  digitalWrite(ledVerde, LOW);
  
  digitalWrite(ledAzul, HIGH);
  
  digitalWrite(ledVermelho, LOW);
  
  delay(1000); // 1 segundo

  // Sinal vermelho
  
  digitalWrite(ledVerde, LOW);
  
  digitalWrite(ledAzul, LOW);
  
  digitalWrite(ledVermelho, HIGH);
  
  delay(5000); // 3 segundos
  
}
