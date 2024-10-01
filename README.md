# trabalhos-de-LIA-2bimestre
trabalhos do segundo bimestre

# Slide 75

![f124cc93-4cb4-4fb9-8abc-cb1187e67b48](https://github.com/user-attachments/assets/039162e8-c34c-4c01-9873-621d7b845cb1)

void setup() {

pinMode(LED_BUILTIN, OUTPUT);

}

void loop() {

digitalWrite(LED_BUILTIN, HIGH);

delay(1000); 

digitalWrite(LED_BUILTIN, LOW);

delay(1000); 

}


# Slide 77

![064da3d2-b059-49bb-b908-2291f600964e](https://github.com/user-attachments/assets/0d9616ac-350e-45ed-935e-bd1de3532160)

const int ledPin1 = 13;

const int ledPin2 = 9;


const int interval = 500;

void setup() {

Serial.begin(9600);


pinMode(ledPin1, OUTPUT);

pinMode(ledPin2, OUTPUT);


Serial.print("LED 1 está conectado ao pino ");

Serial.println(ledPin1);

Serial.print("LED 2 está conectado ao pino ");

Serial.println(ledPin2);

}

void loop() {
   
       
digitalWrite(ledPin1, HIGH); 
      
digitalWrite(ledPin2, LOW);
        
Serial.println("LED 1 aceso, LED 2 apagado");
    
delay(interval);
   
digitalWrite(ledPin1, LOW);
       
digitalWrite(ledPin2, HIGH);
       
Serial.println("LED 1 apagado, LED 2 aceso");
   
delay(interval);
 
  }

# Slide 80

![2eddd95e-b496-4640-87fd-2ef4d6f119d0](https://github.com/user-attachments/assets/da3f47a6-9d96-4faa-bbb1-d293cc245ec7)

const int ledPin1 = 4;

const int ledPin2 = 5;

const int ledPin3 = 6;

void setup() {

pinMode(ledPin1, OUTPUT);

pinMode(ledPin2, OUTPUT);

pinMode(ledPin3, OUTPUT);

}

void loop() {

digitalWrite(ledPin1, HIGH);

delay(1000);

digitalWrite(ledPin1, LOW);


digitalWrite(ledPin2, HIGH);

delay(1000);

digitalWrite(ledPin2, LOW);


digitalWrite(ledPin3, HIGH);

delay(1000);

digitalWrite(ledPin3, LOW);

}

# Slide 82

![b7826ab7-7a2e-4262-b62b-985a901f639b](https://github.com/user-attachments/assets/caccd2e7-a518-46cb-ae0f-9e8f14192851)

const int buttonpin = 2;

const int ledpin = 13;

int buttonState = 0;

void setup() {

pinMode(buttonPin, OUTPUT);

pinMode(buttonPin, INPUT);

}

void loop() {

buttonState = digitalRead(buttonPin);


if buttonState == HIGH {

digitalWrite(ledpin, HIGH);

} else {

digitalWrite(ledPin, LOW);

}

# Slide 83

![f90fc72c-1849-4883-a49e-fb565a49e459](https://github.com/user-attachments/assets/843f2b24-b750-4a59-8129-92bab94541ae)

const int buttonpin = 2;

const int ledpin = led_BUILTIN;


int buttonPushCounter = 0;

int buttonState = 0;

int lastButtonState = 0;


void setup() {

pinMode(buttonPin, INPUT);

pinMode(ledPin, OUTPUT);

Serial.begin(9600);

}

void loop() {

buttonState = digitalRead(buttonPin);

if (buttonState != lastButtonState) {

if (buttonState == HiGH) {

buttonPushConter++;

serial.println("on");

serial.println(number of button pushes:);

serial.println(buttonPushCounter);

} else {


Serial.println("off");

}

delay(50);

}

lastButtonState = buttonState;

}

# Slide 84

int pushButton = 2;


void setup() {

Serial.begin(9600);

pinMode(pushButton, INPUT);


void loop() {

int buttonState = digitalRead(pushButton);

Serial.println(buttonState);

delay(100);

}

