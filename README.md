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
  // Sinal verde - seguir
  digitalWrite(ledVerde, HIGH);
  digitalWrite(ledAzul, LOW);
  digitalWrite(ledVermelho, LOW);
  delay(5000); // 3 segundos

  // Sinal azul (atenção)
  digitalWrite(ledVerde, LOW);
  digitalWrite(ledAzul, HIGH);
  digitalWrite(ledVermelho, LOW);
  delay(1000); // 1 segundo

  // Sinal vermelho - parar
  digitalWrite(ledVerde, LOW);
  digitalWrite(ledAzul, LOW);
  digitalWrite(ledVermelho, HIGH);
  delay(5000); // 3 segundos
}
