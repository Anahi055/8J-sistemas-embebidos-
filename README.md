# 8J-sistemas-embebidos-
Salazar Jaime Lizbeth Anahi 
https://www.tinkercad.com/things/bCWbg7w1QEn/editel
Este es un. enlace para un simulador de sistema embebido 
// C++ code
//
void setup()
{
  Serial.begin(9600);
  pinMode(4, OUTPUT);
}

void loop()
{
  int Val = analogRead(A2);
  Serial.println(Val);
  if (Val < 500) {
    digitalWrite(4, LOW);
  }
  else {
    digitalWrite(4, HIGH);
  }
}
