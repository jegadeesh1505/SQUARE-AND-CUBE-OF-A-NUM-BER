# SQUARE AND CUBE OF A NUMBER
# 8051 Square  Program

## AIM
To write and execute an Assembly language program for finding the square of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value to Port 0 (P0).
3. Execute the program.
4. The output square value is stored in Port 2 (P2).

## PROGRAM
```
 ORG 00H
 MOV DPTR,#4500H
 MOVX A,@DPTR
 MOV B,A
 MUL AB
 INC DPTR
 MOVX @DPTR,A
 INC DPTR
 MOV A,B
 MOVX @DPTR,A
 END

```

## OUTPUT
<img width="1400" height="564" alt="Screenshot 2025-09-25 084957" src="https://github.com/user-attachments/assets/d2aefdfc-ecda-41e9-a3cb-63a708a4796e" />



## RESULT
Thus, the square of the given data is calculated using 8051 Keil.

# 8051 Cube  Program

## AIM
To write and execute an Assembly language program for finding the cube of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value.
3. Execute the program.
4. The output cube value is stored in a memory location.

## PROGRAM
```
 MOV R0,#50H
 MOV A,@R0
 MOV B,@R0
 MUL AB
 MOV R1,B
 MOV B,@R0
 MUL AB
 MOV 51H,A
 MOV 52H,B
 MOV A,R1
 MOV B,@R0
 MUL AB
 ADD A,52H
 MOV 52H,A
 MOV 53H,A
 MOV A,#00H
 ADDC A,53H
 MOV 53H,A
 END

```


## OUTPUT
<img width="1300" height="521" alt="Screenshot 2025-09-25 085351" src="https://github.com/user-attachments/assets/8ce1b60e-ad38-4c91-9483-14fd32efca8b" />


## RESULT
Thus, the cube of the given data is calculated using 8051 Keil.
