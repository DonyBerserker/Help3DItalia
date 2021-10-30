# marlin-2.0.9.1-runout-sensor-manual-bed-levelling.bin
Firmware precompilato per una Ender 3 Pro che utilizza come scheda una Bigtreetech SKR mini E3 1.2. Rispetto al Marlin vanilla sono state applicate le seguenti modifiche: 

* Abilitato il PID autotune per letto ed hotend
* Abilitato il manual bed mesh levelling su 16 punti. Non richiede il Bl-Touch ma è totalmente manuale
* Abilitato il babystepping
* Abilitato il power-loss recovery
* Sostituito nelle impostazioni di pre-riscaldamento l'ABS con il PTEG
* Abilitato il sensore di filamento sul PIN PC12 (etichettato come PT-DET sulla scheda). Se non utilizzato può essere disabilitato via LCD
* La dimensione del letto è stata impostata già a 235x235
* Abilitato l'assistente per il Bed Tramming (angoli + centro)
* Corrente dei motori già impostata a 550

Il firmware è utilizzato su una Ender 3 Pro che utilizza un clone di un Bondtech BMG Dual Gear, impostate gli step/mm in maniera opportuna per il vostro gruppo estrusore.