Nome: Mayumi Kobayashi

Email: mayumi.kobayashi@hotmail.com  

GitHub ID: https://github.com/MayKobayashi  

R.A.: 3011542413016 



n = 0

print("P | Q | R | S | P→Q | R→S | P∨R | (P→Q)∧(R→S)∧(P∨R) | Q∨S | ((P→Q)∧(R→S)∧(P∨R))→(Q∨S)")

for a in range(0, 2):
    for b in range(0, 2):
        for c in range(0, 2):
            for d in range(0, 2):
                if a == 0:
                    P = "V"
                else:
                    P = "F"

                if b == 0:
                    Q = "V"
                else:
                    Q = "F"

                if c == 0:
                    R = "V"
                else:
                    R = "F"

                if c == 0:
                    S = "V"
                else:
                    S = "F"

                if P == "F" or Q =="V":
                    PQ = "V"
                else:
                    PQ = "F"

                if R == "F" or S =="V":
                    RS = "V"
                else:
                    RS = "F"

                if P == "V" or R =="V":
                    PR = "V"
                else:
                    PR = "F"

                if PQ =="V" and RS == "V":
                    PQRS = "V"
                else:
                    PQRS = "F"
                             
                if PQRS =="V" and PR == "V":
                    PQRSPR = "V"
                else:
                    PQRSPR = "F"

                if Q == "V" or S == "V":
                    QS = "V"
                else:
                    QS = "F"

                if PQRSPR == "F" or QS == "V":
                    DC = "V"
                else:
                    DC = "F"
               
                print(f"{P} | {Q} | {R} | {S} |  {PQ}  |  {RS}  |  {PR}  |          {PQRSPR}         |  {QS}  |          {DC}          ")
                
                if DC == "V":
                    n += 1

#Trabalho finalizado
