# Guardrails Automation (`gau`)

Tredici figure Guardrails e i workflow necessari a instradare processi software, legali, fiscali, di design, architettura, medicina, web e paid media. `grl-automation` porta ogni richiesta da intake e read-only a piano, dry-run, approvazioni, esecuzione osservabile e rollback, senza trasformare un agente in un esecutore autonomo.

Modulo BMad. È una porzione del bundle [Guardrails](https://github.com/mlarese/bmad-module-guardrails):
stesse figure, stesso comportamento, solo l'area automation.

> **Generato.** Questo repository è prodotto da `tools/build_modules.py` nel
> repository [bmad-module-guardrails](https://github.com/mlarese/bmad-module-guardrails).
> Le modifiche si fanno lì e poi si rigenera: qui vengono sovrascritte.

## Figure

| Figura | Ruolo | Skill | Cosa presidia |
| ------ | ----- | ----- | ------------- |
| 🛡️ Vera | Data Protection Officer | `grl-agent-privacy` | Parte sempre dai dati concreti — quali dati personali esattamente, chi li vede, per quanto tempo — e separa l'obbligo GDPR vero dalla prassi diffusa: base giuridica di una… |
| 🔐 Kai | Application Security Engineer | `grl-agent-security` | Pensa come chi attacca e ordina i rischi per probabilità reale, non per gravità teorica; ogni difesa la pesa per quanto costa contro quanto danno evita. |
| ⚖️ Aldo | Tech Lawyer | `grl-agent-legal` | Traduce licenze open source (GPL, AGPL, MIT), proprietà intellettuale del codice — anche quello generato dall'AI — contratti e DPA con i fornitori, termini di servizio e vincoli… |
| 📐 Nils | Regulatory Compliance | `grl-agent-compliance` | Prima esclude, poi prescrive: delle norme che ti preoccupano, quasi sempre metà non ti riguarda. |
| 🧾 Marta | Fiscalista e Finanza Agevolata | `grl-agent-fiscal` | Ricerca fonti fiscali, contabili e di finanza agevolata italiane ed europee, verifica requisiti, scadenze, spese ammissibili e rendicontazione, e traduce tutto in un verdetto… |
| 👁️ Iris | Design Critic | `grl-agent-ui-critic` | Guarda una landing o una schermata e dice subito dove l'ha già vista: hero centrato in gradiente, tre card con icona, Inter a peso 600, blu-viola ovunque. |
| 🧱 Otto | Code Architect | `grl-agent-architecture` | Usa SOLID, KISS, DRY, separazione delle responsabilità, vertical slice e architettura esagonale come attrezzi e mai come dogmi: guarda confini fra moduli, direzione delle… |
| 🖥️ Bruno | Infrastructure & Ops Engineer | `grl-agent-ops` | Sistemista veterano: prima di aggiungere un pezzo di infrastruttura chiede quante persone la manterranno alle tre di notte, e il suo mestiere è toglierne, non aggiungerne — «ti… |
| 🩺 Livia | Clinical Informatics | `grl-agent-health` | Medico che ha passato vent'anni dentro i sistemi informativi sanitari: sa che un farmaco non è una stringa, che una dose senza unità di misura è un errore in attesa, e che il… |
| 🧠 Enzo | AI Engineer | `grl-agent-ai` | Costruisce applicazioni che usano modelli linguistici e sa soprattutto quando non servono: metà delle funzioni per cui viene chiamato si risolvono con una query, una regola o un… |
| 🧩 Milo | WordPress Component Architect | `grl-agent-wordpress` | Progetta e implementa WordPress a componenti con Gutenberg, Elementor, ACF, campi custom, template e Media Library, senza lasciare contenuti strutturati dentro pagine monolitiche… |
| 🔎 Nora | SEO Strategist & Search Systems Auditor | `grl-agent-seo` | Distingue domanda, intento, crawl, indicizzazione, contenuto, dati strutturati e misurazione, verifica sempre live le regole SEO e trasforma ogni diagnosi in una modifica… |
| 📣 Dalia | Media Manager & Paid Advertising Strategist | `grl-agent-ads` | Trasforma un obiettivo commerciale in campagne pagate misurabili: Google Ads, Search, Performance Max, Display, YouTube e gli altri canali ADV entrano solo con destinatario,… |

## Skill e workflow

| Skill | Comando | Cosa fa |
| ----- | ------- | ------- |
| `gau-profile` | Profila il progetto | Raccoglie in pochi minuti gli otto campi che danno contesto a tutte le figure, criticità inclusa. |
| `gau-profile` | Aggiorna il profilo | Riallinea il profilo quando il progetto cambia, e dice se il cambiamento invalida rischi già accettati. |
| `gau-board` | Convoca il collegio | Fa leggere lo stesso artefatto alle sole figure pertinenti e restituisce un riepilogo unico, conflitti compresi. |
| `gau-board` | Rischi già accettati | Mostra, raggruppato per figura, quello che il progetto ha consapevolmente scelto di accettare. |
| `gau-board` | Gate di rilascio | Verifica una release identificata e restituisce GO, GO_CON_CONDIZIONI, NO_GO o EVIDENZA_INSUFFICIENTE. |
| `grl-legal-updates` | Ultime novità legali | Recupera leggi, decreti, bollettini, sentenze ed emendamenti nel periodo indicato, con ricerca live, matrice di copertura, lineage di vigenza e due gate bmad-review. |
| `grl-fiscal-updates` | Ultime novità fiscali | Recupera norme fiscali, circolari, bollettini, emendamenti, bandi e incentivi nel periodo indicato, con ricerca live, matrice di copertura, lineage di vigenza e due gate bmad-review. |
| `grl-mdsw` | È un dispositivo medico? | Verifica se una funzione software ha una finalità medica su un singolo paziente, distingue archiviazione e visualizzazione da interpretazione clinica e indica se rientra nel MDR e in quale classe (I, IIa, IIb, III), con l'impatto sul piano. Non produce certificazione. |
| `grl-web` | Crea una landing o un sito | Dal brief di conversione — destinatario, promessa, obiezione, prova, azione — al mockup HTML a file singolo. |
| `grl-web` | Riprendi un mockup | Rientra su una pagina già fatta, applica il cambiamento e segnala se contraddice una decisione già registrata. |
| `grl-web` | Diagnostica una pagina | Perché una pagina che esiste già non converte: il brief ricostruito all'indietro e da tre a cinque mosse concrete. |
| `grl-web` | Promuovi a progetto | Dal mockup approvato al sito vero: Tailwind da CLI standalone, SEO, form, accessibilità, pronto per il deploy. |
| `grl-web` | Configura un sito vero | Prepara la scheda di un sito con parti condivise, contenuti che cambiano e animazioni; la scheda può poi passare a bmad-spec per essere trasformata in fette per bmad-build. |
| `grl-ads` | Audita account e campagne | Legge export e report, definisce il perimetro e ordina blocchi, distorsioni e opportunità senza modificare l'account. |
| `grl-ads` | Prepara un piano media | Dall'obiettivo alla struttura delle campagne, agli asset, al budget come scenario e al piano di misura. |
| `grl-ads` | Verifica tracking e consenso | Mappa eventi, conversioni, tag, fonte, consenso e verifiche senza caricare dati personali. |
| `grl-ads` | Ottimizza con change set | Confronta periodi compatibili e propone modifiche a campagne e budget con soglie, approvazione, dry-run e rollback. |
| `grl-ads` | Preflight della campagna | Controlla tracking, destinazione, claim, asset, policy, consenso, budget, autorizzazioni e rollback prima dell'azione. |
| `grl-ads` | Applica un change set | Esegue solo un'azione esplicitamente autorizzata, delimitata e validata; altrimenti resta in awaiting_approval o blocked. |
| `grl-automation` | Instrada un'automazione | Classifica lo scenario, sceglie agenti e workflow BMad e dichiara capability mancanti, scope e approvazioni. |
| `grl-automation` | Prepara un piano eseguibile | Costruisce passi idempotenti con input, output, precondizioni, rischio, approvazione e rollback. |
| `grl-automation` | Esegui controlli read-only | Raccoglie evidenze e confronti riproducibili senza modificare sistemi esterni. |
| `grl-automation` | Prepara un dry-run | Genera e valida diff o payload senza spendere, pubblicare o applicare side effect. |
| `grl-automation` | Esegui dopo approvazione | Applica solo lo scope approvato, registra prima/dopo e osserva il risultato; in caso di errore attiva il rollback. |
| `grl-automation` | Riprendi un'automazione | Riprende un run esistente dal primo passo non concluso senza duplicare scritture o side effect. |

## Installazione

```
bmad install gau
```

Poi, come primo passo, `gau-profile`: raccoglie il profilo di progetto — settore,
dati trattati, mercato, stack, criticità — e da lì ogni figura deriva quanto essere
severa. Senza profilo il default resta `normal` e le figure partono senza contesto.

## Memoria condivisa

Il profilo vive in `{project-root}/_bmad/memory/grl-shared/project-profile.md`, insieme
a `decisions.md` e `accepted-risks.md`. Il percorso è lo stesso per tutti i moduli
Guardrails: installandone due, il profilo resta uno solo e si compila una volta.

## Convivenza con il bundle

Questo modulo installa skill con **lo stesso nome** del bundle `grl` — `grl-agent-privacy`
sta identica in entrambi. Bundle e moduli tematici non vanno installati insieme nello
stesso progetto: si sceglie il bundle completo, oppure i moduli delle aree che servono.

## Licenza

MIT.
