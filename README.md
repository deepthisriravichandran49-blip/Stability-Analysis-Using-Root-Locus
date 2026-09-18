# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software
## Theory:
<img width="1828" height="3112" alt="image" src="https://github.com/user-attachments/assets/663916fd-32f9-46e7-b4bc-8ad13585644e" />
<img width="1856" height="3008" alt="image" src="https://github.com/user-attachments/assets/3f15b42b-3fe2-4f28-8b6d-dcc8c5178856" />
<img width="1784" height="920" alt="image" src="https://github.com/user-attachments/assets/0bf447c5-94ab-4863-8fd2-626fd471740f" />

## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 
```
num=[1];
den=[1 15 50 0];
sys=tf(num,den);
rlocus(sys);
[k,poles]=rlocfind(sys)
```
## Output:
<img width="1913" height="1035" alt="image" src="https://github.com/user-attachments/assets/32e892bf-d8ae-401b-ac98-fb7de56d4a83" />
<img width="1065" height="326" alt="image" src="https://github.com/user-attachments/assets/89a4b4d5-3074-4f37-ab46-143712ba0e5c" />
<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/38d7d77a-69ec-4eb3-997d-8a654295c1b8" />

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 755.9205.
