# 📊 Churn Prediction: Detailná Analytická Štruktúra Projektu s AI
## Predikcia Odchodu Zákazníkov v Telekomunikačnom Sektore

**Cieľ Projektu:**
Cieľom tohto projektu je vyvinúť a demonštrovať štruktúrovaný prístup k vytvoreniu modelu umelej inteligencie (Machine Learning), ktorý dokáže predpovedať, ktorí zákazníci O2 sú s najväčšou pravdepodobnosťou náchylní na odchod (churn). Včasná identifikácia umožní proaktívne zásahy a optimalizáciu retencia kampaní.

---

### Prečo je Projekt Kritický pre Biznis (O2):

* **Zníženie Odlivu:** Udržanie existujúcich zákazníkov je nákladovo efektívnejšie ako získavanie nových.
* **Optimalizácia Nákladov:** Cielené retencia kampane sú efektívnejšie, pretože sa zameriavajú len na vysoko rizikových zákazníkov.
* **Lepšie Porozumenie Zákazníkom:** Analýza faktorov (Feature Importance) vedúcich k odchodu poskytuje cenné insights o slabých miestach služieb.
* **Môj Záujem o AI:** Projekt aplikuje techniky strojového učenia na reálny biznis problém a rozvíja moje zručnosti v AI dátovej analytike.

---

## Navrhovaná Štruktúra a Fázy Projektu (Metodický Prehľad)

### Fáza 1: Zber a Predspracovanie Dát (SQL & Dátová Integrita)

* **Zdroj Dát (Hypotetické):** Dáta o zákazníkoch z rôznych interných systémov (CRM, Fakturácia, Podpora).
    * **Zákaznícke demografické údaje:** Vek, lokalita, typ zákazníka.
    * **História využívania služieb:** Dĺžka trvania zmluvy, priemerná mesačná spotreba (hlas, dáta, SMS), využívanie TV služieb.
    * **Interakcie so zákazníckou podporou:** Počet volaní, typy problémov, dĺžka riešenia.
    * **Fakturačné údaje:** Spôsob platby, história platieb.
    * **Dáta o zariadeniach:** Typy vlastnených zariadení (ak sú evidované).
* **Čistenie a Transformácia Dát:** Riešenie chýbajúcich hodnôt, detekcia anomálií, normalizácia/škálovanie dát (základné zručnosti pre Data Analyst).
* **Vytváranie Vlastností (Feature Engineering):** Extrahovanie nových, relevantných premenných z existujúcich dát.
    * *Príklad:* Priemerná spotreba za posledné 3 mesiace, zmena spotreby oproti predchádzajúcemu obdobiu, počet sťažností za štvrťrok.
    * *Cieľová Premenná:* Vytvorenie binárnej premennej **"Churn"** (1 ak zákazník odišiel, 0 ak zostal).

### Fáza 2: Exploratívna Dátová Analýza (EDA)

* **Vizualizácia Dát:** Grafy a tabuľky na pochopenie distribúcie dát a vzťahov medzi premennými (s využitím Power BI/Excel/Python).
* **Identifikácia Kľúčových Faktorov:** Vyhľadanie dátových vzorcov a trendov, ktoré naznačujú náchylnosť na odchod.
* **Korelácia:** Pochopenie vzájomných závislostí medzi rôznymi premennými.

### Fáza 3: Výber a Tréning AI Modelu (Machine Learning)

* **Rozdelenie Dát:** Rozdelenie dát na trénovaciu a testovaciu množinu (napr. 70/30).
* **Výber Algoritmov:** Zváženie algoritmov vhodných pre klasifikáciu a interpretovateľnosť.
    * *Príklady:* Logistická regresia (základ), Rozhodovacie stromy, Náhodné lesy (Random Forests), Gradient Boosting (XGBoost).
* **Tréning Modelu:** Trénovanie vybraných modelov na trénovacej množine dát.
* **Hyperparameter Tuning:** Optimalizácia parametrov modelu pre dosiahnutie najlepšieho výkonu.

### Fáza 4: Vyhodnotenie Modelu a Interpretácia Výsledkov

* **Metriky Výkonu:** Vyhodnotenie modelov na testovacej množine pomocou relevantných metrík.
    * *Pre Churn je kľúčový:* **Recall** (identifikovať čo najviac odchádzajúcich zákazníkov) a **Precision** (minimalizovať falošné pozitiva), F1-skóre, AUC-ROC krivka.
* **Interpretácia Modelu (Feature Importance):** Pochopenie, ktoré vlastnosti dát majú najväčší vplyv na predikciu odchodu zákazníka (napr. Dĺžka trvania zmluvy, počet sťažností).
* **Vizualizácia Výsledkov:** Prezentácia výkonu modelu a kľúčových zistení (napr. Confusion Matrix) pre Biznis Stakeholderov.

### Fáza 5: Nasadenie a Monitorovanie (Návrh Pre Produkciu)

* **Pravidelné Dátové Pipeline:** Návrh procesu, ako by sa model pravidelne aktualizoval novými dátami (práca Data Analysta/Engineera).
* **Integrovanie do Systémov:** Návrh, ako by sa predikcie modelu integrovali do CRM systémov alebo marketingových nástrojov pre cielené kampane.

---

### **Potenciálne Rozšírenia (Ukážka Inovácie):**

* **Segmentácia zákazníkov:** Využitie clusteringu na identifikáciu rôznych skupín zákazníkov náchylných na odchod s odlišnými charakteristikami.
* **Využitie NLP:** Analýza textových dát zo sťažností alebo chatov pre lepšie pochopenie sentimentu zákazníkov.

  Pre detailnú analytickú štruktúru projektu (Hypotetické dáta, EDA, Výber Modelu, Metriky), prosím, prejdite na dokument:

**[Detailná Analytická Štruktúra: Churn Prediction >](Churn_Prediction_Detailed_Analysis.md)**
