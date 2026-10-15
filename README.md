# 🎙️ Autonomous Event-Based Audio Recording System (Raspberry Pi 5 HAT)

Kompletný hardvérový a softvérový návrh autonómneho, udalosťami riadeného (event-based) audiozáznamníka pre dlhodobé nasadenie v teréne. Projekt vznikol ako bakalárska práca na **FEKT VUT v Brne** (odbor *Audio inžinierstvo*).

📄 **[Prečítať kompletný text bakalárskej práce (PDF so schémami a meraniami)](./Bakalarska_praca_Hrobak.pdf)**

---

## 🛠️ Prehľad projektu (HW + SW)

Cieľom projektu bolo navrhnúť, vyrobiť a oživiť rozširujúci hardvérový modul (**PCB HAT**) pre platformu **Raspberry Pi 5** spolu s obslužným softvérom, ktorý umožňuje spoľahlivý, udalosťami spúšťaný záznam zvuku v teréne bez nutnosti neustáleho dohľadu.

### 1. Hardvérová časť (PCB Design: Eagle ➔ KiCad)
* **Vlastný PCB HAT modul:** Navrhnutý priamo pre 40-pinové rozhranie Raspberry Pi 5.
* **Iteratívny vývoj (2 revízie):** 
  * *Revízia 1:* Prvotný prototyp navrhnutý v prostredí **Autodesk Eagle** na overenie konceptu.
  * *Revízia 2:* Kompletný redizajn a optimalizácia layoutu v prostredí **KiCad** na základe praktických meraní a testov prvej verzie.
* **Realizácia:** Samostatný výber súčiastok (BOM), príprava výrobných Gerber dát, osadenie a oživenie prototypu (HW bring-up).

### 2. Softvérová časť (Firmware / Embedded Linux)
* **Event-Based architektúra:** Softvér neukladá prázdne ticho, ale priebežne vyhodnocuje vstupný audio signál a spúšťa záznam pri detekcii relevantnej akustickej udalosti.
* **Autonómna prevádzka:** Automatická správa úložiska, logovanie stavov systému a odolnosť voči výpadkom pri dlhodobom nasadení v teréne.

---

## 📸 Ukážka hardvéru a schémy
*(Tip pre Lukáša: Ak do repozitára nahráš fotku dosky pod názvom `pcb_photo.jpg`, odkomentuj riadok nižšie a zobrazí sa priamo tu!)*

<!-- ![PCB HAT pre Raspberry Pi 5](./pcb_photo.jpg) -->

---

## 👤 Autor
**Bc. Lukáš Hrobák**  
* Bakalárske štúdium: FEKT VUT v Brne – Audio inžinierstvo (2023 – 2026)
* Magisterské štúdium: FEL ČVUT v Prahe – Komunikace a internet věcí (2026 – súčasnosť)