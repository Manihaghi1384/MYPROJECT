int buzzer = 8;
int reedswitch = 10;

void setup() {
  pinMode(buzzer, OUTPUT);      
  pinMode(reedswitch, INPUT);   
}

void loop() {
  if (digitalRead(reedswitch) == LOW) {  
    digitalWrite(buzzer, HIGH);           
    }
  else {
    digitalWrite(buzzer, LOW);            
  }
}
