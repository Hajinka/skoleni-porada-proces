```mermaid
flowchart LR

%% ───────────── LANES ─────────────
subgraph L1["Ředitel / Statutár"]
  direction TB
  E0((Start))
  T1([Vznik potřeby strategické porady])
  T2([Stanovení termínu porady])
  T3([Stanovení programu porady])
  T6([Zahájení porady])
  T8([Řízení diskuse])
  T11([Ukončení porady])
  E1((End))
  T13([Neformální kontrola plnění úkolů])
end

subgraph L2["Vedoucí projektů / týmů"]
  direction TB
  T4([Potvrzení účasti])
  T5([Příprava témat z vlastní agendy])
  T7([Prezentace stavu projektů])
  T12([Převzetí úkolů])
  T14([Plnění úkolů dle aktuálních priorit])
end

subgraph L3["Členové týmu"]
  direction TB
  T4b([Zapsání termínu do kalendáře])
  T6b([Příchod na poradu])
  T10([Účast v diskusi])
  T12b([Převzetí dílčích úkolů])
  T15([Plnění úkolů dle kapacit])
end

%% ───────────── FLOW ─────────────
E0 --> T1 --> T2 --> T3
T3 --> T4
T3 --> T4b
T4 --> T5

T4b --> T6b --> T6
T6 --> T7 --> T8 --> T10 --> T11 --> E1

T11 --> T12 --> T14 --> T13
T11 --> T12b --> T15 --> T13

