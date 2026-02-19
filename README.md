```mermaid
flowchart LR

%% ───────────── SWIMLANES ─────────────
subgraph L1["Ředitel / Statutár"]
    A1[Vznik potřeby strategické porady<br/>(pravidelný měsíční cyklus)]
    A2[Stanovení termínu porady]
    A3[Stanovení programu porady]
    A6[Zahájení porady]
    A8[Řízení diskuse]
    A11[Ukončení porady]
    A13[Neformální kontrola plnění úkolů]
end

subgraph L2["Vedoucí projektů / týmů"]
    B1[Potvrzení účasti]
    B2[Příprava témat z vlastní agendy]
    B4[Prezentace stavu projektů]
    B6[Vstup do detailní diskuse]
    B9[Převzetí úkolů]
    B11[Plnění úkolů dle aktuálních priorit]
end

subgraph L3["Členové týmu"]
    C1[Zapsání termínu do kalendáře]
    C2[Příchod na poradu]
    C4[Účast v diskusi]
    C6[Převzetí dílčích úkolů]
    C8[Plnění úkolů dle kapacit]
end

%% ───────────── TOK PROCESU ─────────────

%% Vznik potřeby
A1 --> A2 -->
