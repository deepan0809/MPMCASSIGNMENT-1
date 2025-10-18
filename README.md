# MPMCSKILL_ASSESSMENT1
# FACTORIAL-OF-A-NUMBER_STORES DATA
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To Write an assembly language program in 8051 to find the factorial of a given  number and store the result in memory.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

### Algorithm

1. Start the program
2. Set DPTR = 4500H
3. Read number N from memory (4500H) into A
4. Move A → R0 (store N in R0)
5. Set A = 1 (initialize result)
6. Repeat:

   * Move R0 → B
   * Multiply A × B → result in A
   * Decrement R0
   * If R0 ≠ 1, repeat loop
7. Increment DPTR (to 4501H)
8. Store result (A) to memory (4501H)
9. Stop the program



---

## FLOWCHART
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/b9d94eea-a743-43f4-ac56-fba678ae2f81" />



---

## PROGRAM
```asm
ORG 0000H
789yuMOV DPTR,#4500H     
MOVX A,@DPTR        
MOV R0,A            
MOV A,#01H          
FACT_LOOP:
    MOV B,R0        
    MUL AB         
    DEC R0         
    CJNE R0,#01H,FACT_LOOP  
INC DPTR           
MOVX @DPTR,A        
SJMP $              
END


```
OUTPUT

<img width="1926" height="1086" alt="image" src="https://github.com/user-attachments/assets/a2e2663a-c004-428e-8bb2-94d1e943fde7" />


<img width="1926" height="265" alt="image" src="https://github.com/user-attachments/assets/b407e7bf-8b7a-4d2e-a3a8-29628279467f" />


---
MANUAL CALCULATIONS
![WhatsApp Image 2025-09-24 at 22 50 46_011089e3](https://github.com/user-attachments/assets/0a9fbf9e-5636-4914-9723-2df721668f67)

---

RESULT

Thus, the factorial of a number was calculated and executed and stored successfully using 8051 Keil.

---


