# ClaudeXLaura: agente esperto PPWR

Agente Claude Code specializzato sul **Regolamento (UE) 2025/40 sugli imballaggi e i rifiuti di imballaggio (PPWR)**, con focus sull'**Allegato VII** (valutazione della conformità e documentazione tecnica, il "fascicolo tecnico").

## Come si usa
In Claude Code, in questo repository:
- chiedi direttamente, per esempio: *«Usa l'agente ppwr-esperto: cosa deve contenere il fascicolo tecnico di una vaschetta in PET per alimenti?»*
- oppure scrivi `@ppwr-esperto` seguito dalla domanda.

Cose che sa fare:
- rispondere su qualsiasi articolo o allegato, citando il testo ufficiale;
- redigere un fascicolo tecnico (All. VII) e una Dichiarazione di conformità UE (All. VIII) partendo dai modelli;
- revisionare un fascicolo o una DoC esistenti, segnalando le lacune;
- mappare TDS, SDS, DoC MOCA, certificazioni e test di laboratorio sui requisiti PPWR;
- produrre scadenzari e gap analysis per ruolo (fabbricante, fornitore, importatore, distributore).

## Struttura
| Percorso | Contenuto |
|---|---|
| `.claude/agents/ppwr-esperto.md` | Definizione dell'agente (istruzioni e regole) |
| `ppwr/fonti/PPWR_Reg_UE_2025-40_IT.txt` | Testo integrale ufficiale IT (GU L 22.1.2025) |
| `ppwr/00-indice.md` | Indice di articoli e allegati con numero di riga |
| `ppwr/01-allegato-VII-fascicolo-tecnico.md` | Studio approfondito dell'Allegato VII e di tutti i suoi rinvii |
| `ppwr/02-sintesi-obblighi-e-scadenze.md` | Date, valori numerici, obblighi per ruolo |
| `ppwr/modelli/` | Modello di fascicolo tecnico e di DoC UE |

## Tenerlo aggiornato
Quando escono atti delegati o di esecuzione (es. art. 7(8) sul formato della documentazione tecnica, art. 6(4) sui criteri di riciclabilità), linee guida della Commissione o norme armonizzate, salva il testo in `ppwr/fonti/`. L'agente li consulta automaticamente.

> L'agente fornisce supporto tecnico-normativo e non sostituisce una consulenza legale.
