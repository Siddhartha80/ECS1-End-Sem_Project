# ECS1-End-Sem_Project

Question-1
Implement the four Boolean functions listed using three half-adder circuits. 
D = A xor B xor C 
E = A'BC+ AB'C 
F = ABC' + (A'+B') C
G = ABC

![image](https://github.com/Siddhartha80/ECS1-End-Sem_Project/assets/133953774/ab3ab130-31ce-488f-8bbe-45fec84ab4be)

![image](https://github.com/Siddhartha80/ECS1-End-Sem_Project/assets/133953774/88ac9892-2583-470c-b848-fc1187c96838)

Truth Table


![image](https://github.com/Siddhartha80/ECS1-End-Sem_Project/assets/133953774/15ff8b4e-77d7-43cf-a281-a1a6cf1fc39e)

Code:
CHIP ThreeHalfAdders{
      IN  a, b, c;
    OUT sum,   
        carry; 
    PARTS:
    HalfAdder(a=a,        b=b,    sum=axorb,          carry=ab);
    HalfAdder(a=axorb, b=c,    sum=d,   carry=e);
    HalfAdder(a=c,        b=ab,  sum=f,        carry=g);
}


