# MICROMAUSE
way to study the micromaus
//Перший етап Мікромауса
const int FwdPin_A = 6; 
const int BwdPin_A = 8;  
const int FwdPin_B = 10; 
const int BwdPin_B = 12;  

int MaxSpd = 10;
void setup() {
pinMode(FwdPin_A, OUTPUT);
pinMode(BwdPin_A, OUTPUT);
pinMode(FwdPin_B, OUTPUT);
pinMode(BwdPin_B, OUTPUT);
}
void loop() {
digitalWrite(BwdPin_A,LOW);
digitalWrite(BwdPin_B,LOW);
digitalWrite(FwdPin_A,MaxSpd);
digitalWrite(FwdPin_B,MaxSpd);
delay (2000);
digitalWrite(FwdPin_A,LOW);
digitalWrite(FwdPin_B,LOW);
delay (2000);

digitalWrite(FwdPin_A,MaxSpd);
digitalWrite(FwdPin_B,MaxSpd);
delay (2000);
digitalWrite(FwdPin_A,LOW);
digitalWrite(FwdPin_B,LOW);
delay (2000);
}    
