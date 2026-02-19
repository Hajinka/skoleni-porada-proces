```mermaid
flowchart LR

subgraph L1["Ředitel / Statutár"]
  direction TB
  E0(("Vznik potřeby strategické porady"))
  T1(["Stanovení termínu porady"])
  T2(["Stanovení programu porady"])
  T3(["Příprava podkladů na poradu"])
  T4(["Zahájení porady"])
  T5(["Projednání jednotlivých bodů programu"])
  T8(["Definování úkolů s termíny pro členy týmu"])
  T9(["Stanovení termínu další porady"])
  E1(("Ukončení porady"))
end

E0 --> T1 --> T2 --> T3 --> T4 --> T5 --> T8 --> T9 --> E1
