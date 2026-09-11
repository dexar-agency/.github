# Come si contribuisce

Regole essenziali, valide in tutti i repository dell'organizzazione:

1. **Ogni lavoro parte da una issue.** Se non c'è una issue, il lavoro non
   esiste. Usa il template: dice cosa succede, cosa dovrebbe succedere, chi
   lo chiede e che impatto ha.
2. **Mai lavorare su `main` o su `dev`.** Si lavora su un branch dedicato,
   il cui nome dice il lavoro (es. `fix/form-contatti-validazione`).
   (Chi ha la responsabilità dei rilasci ha una corsia propria, descritta
   nel repository `governance`.)
3. **Il branch torna con UNA pull request verso `dev`** (una per lavoro,
   mai una per pezzo), con `Closes #N` nella descrizione. La pipeline deve
   essere verde; la PR viene mergiata in squash dopo la review.
4. **La promozione `dev` → `main` è un atto separato**, riservato a chi ha
   la responsabilità del rilascio: un fast-forward dello stesso commit già
   verificato, mai una seconda pull request; `dev` e `main` restano identici.
5. **Mai credenziali nel codice** — nemmeno in file di appoggio o di
   backup. Un controllo automatico blocca le PR che ne contengono.

Il dettaglio completo del flusso, le policy di accesso e le procedure per
gli incidenti sono nel repository privato `governance` (chi lavora con noi
vi ha accesso).
