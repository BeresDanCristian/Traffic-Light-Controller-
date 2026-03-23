# Traffic Light Controller
# Traffic Light Controller - Basys 3 FPGA

Acest proiect implementează un sistem de control pentru semafoare (intersecție), dezvoltat în **Vivado** și testat pe placa de dezvoltare **Basys 3**. Proiectul utilizează logica automatelor de stare (FSM) pentru a gestiona secvențele de culori și temporizarea acestora.

## 🚦 Descrierea Proiectului
Sistemul simulează controlul traficului într-o intersecție, gestionând stările standard: **Verde**, **Galben** și **Roșu**. Logica este implementată în Verilog/VHDL, având la bază o diagramă de stări bine definită care asigură tranziții sigure și timpi de așteptare optimizați.

## 🛠️ Specificații Tehnice
* **Platformă Hardware:** Basys 3 (Xilinx Artix-7).
* **Software de Proiectare:** Vivado 2024.2.
* **Logica de Control:** Automat de stare finit (Finite State Machine - FSM).
* **Resurse utilizate:** * Ceasul intern al plăcii pentru temporizare.
    * LED-urile integrate pentru vizualizarea stărilor semaforului.
    * Switch-uri/Butoane pentru reset sau moduri de urgență.

## 📊 Logică și Funcționare
Conform diagramei de stare incluse în proiect, sistemul parcurge următoarele etape:
1. **State_Green:** Permite circulația pe direcția principală.
2. **State_Yellow:** Tranziție securizată pentru pregătirea opririi.
3. **State_Red:** Oprirea traficului pentru a permite trecerea pe cealaltă direcție/pietoni.

## 📂 Structură Folder Hardware
Fișierul de constrângeri (`Basys3_Master.xdc`) este configurat pentru a mapa ieșirile logice ale proiectului pe pinii fizici ai FPGA-ului, asigurând legătura corectă cu LED-urile și perifericele plăcii.

---
**Autori:** * Bereş Dan-Cristian  
* Nemeţi Crişan Alexandru Denis  

**Grupa:** 2133/3  
**Instituție:** Universitatea Tehnică din Cluj-Napoca (ETTI)
