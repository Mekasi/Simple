#define pir 3
#define rel 5
#define fr A0

void setup() {

pinMode(pir, INPUT);
pinMode(rel, OUTPUT);
pinMode(fr, INPUT);
}

void loop()
{
if ((digitalRead(pir) == HIGH) && (analogRead(fr) < 400)) {
digitalWrite(rel, HIGH);
} else {
digitalWrite(rel, LOW);
};
}
