# CODIGO02-PROFESSOR

void firstEffect (void);
void secondEffect (void);

void setup()
{    
  DDRB = 0x9;
}

int option = HIGH;

void loop()
{
    
  switch (option)
  {
    case HIGH:
      firstEffect();
      break;
    case LOW:
      secondEffect();
      break;
  } 
   option=!option;
 
}
void firstEffect (void)
{
  PORTB = 0x0;
  delay(1000);
  
  PORTB = PORTB | 0x7; //função ou
  delay(1000);
 
}
  void secondEffect (void)
{
    PORTB = 0x0;
    delay(1000);
    PORTB = 0x2;
  delay(1000);
}


segundooo
void setup()
{    
  DDRB = 0xB111111;
}

void loop()
{
    
  PORTB = 0x0;
  delay(1000);
  
  //PORTB |= 0B001111; //função ou
  
  PORTB |= (1<<2); //desloque o bit 1 4 vezes para a esquerda 
  delay(1000);
 
}




terceiro
void firstEffect (void);

void setup()
{    
  DDRB = 0x9;
}

void loop()
{
    
  firstEffect();
 
}
void firstEffect (void)
{
  
  for (int i = 0; i<3 ; i++)
  {
    PORTB = 0x0;
    delay(200);

    PORTB |= (1<<i);
    delay(200);
  
  }
}

 
