#define redled 3
#define yellowled 5
#define greenled 6
#define whiteled 2
#define button 4
#define Start 7

int KondisiButton =0;
int KondisiStart =0;

void setup()
{
  Serial.begin(9600);
  pinMode(redled, OUTPUT);
  pinMode(yellowled, OUTPUT);
  pinMode(greenled, OUTPUT);
  pinMode(button, INPUT_PULLUP);
  pinMode(Start, INPUT_PULLUP);
  
}

void loop()
{
  buttonState();
  KondisiStart = digitalRead(Start);
  
  if(KondisiStart == LOW){
  Serial.println("Start");
  digitalWrite(redled, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(redled, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  
  digitalWrite(yellowled, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(yellowled, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  
  digitalWrite(greenled, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(greenled, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  Serial.println("finish");
  delay(1000);
  }
  
  else{
    return;
  }
}

void buttonState()
{
  KondisiButton = digitalRead(button);
  
  if(KondisiButton == LOW){
    digitalWrite(whiteled, HIGH);
  }
  else{
    digitalWrite(whiteled, LOW);
  }
  
}
