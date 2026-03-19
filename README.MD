# Perché questo layout è meglio delle alternative per scrivere in italiano?
Non lo è. Personalmente lo trovo più adatto rispetto alle alternative,
ma ciò non implica che sia migliore per qualche ragione oggettiva.

Questo layout è presente nativamente su Linux, è un banale porting.

L'alternativa che viene solitamente proposta è il layout Americano internazionale.

Le motivazioni per cui penso sia superiore per la scrittura in lingua italiana sono:
- Assenza di "dead-keys", che rallentano pesantemente la scrittura
- Tutte le lettere accentate sono nel terzo livello (alt destro su Windows/Linux, Option su macOS).

Per fare le lettere accentate, basterá fare ALT destro + lettera (su Windows/Linux) oppure Option (⌥) + lettera (su macOS).

# Ma quindi come si fanno le accentate non ho capito bro

Su **Windows/Linux** si usa ALTGR, su **macOS** si usa Option (⌥). Il funzionamento è identico:

| Combinazione (Windows/Linux) | Combinazione (macOS) | Risultato |
| ---------------------------- | -------------------- | --------- |
| ALTGR + a | Option + a | à |
| ALTGR + e | Option + e | è |
| ALTGR + i | Option + i | ì |
| ALTGR + o | Option + o | ò |
| ALTGR + u | Option + u | ù |
| ALTGR + z | Option + z | á |
| ALTGR + d | Option + d | é |
| ALTGR + k | Option + k | í |
| ALTGR + l | Option + l | ó |
| ALTGR + j | Option + j | ú |

Quindi, banalmente, ALTGR/Option + vocale fa la lettera con l'accento grave, mentre premere la lettera esattamente sotto ne fa la versione con l'accento acuto.

## Ok ma se voglio fare l'accentata maiuscola cosa devo fare scusa
Esattamente la stessa combinazione fatta qui sopra, ma tenendo premuto SHIFT oppure inserendo CAPS LOCK.

## Ok bro penso di aver capito ma se ALTGR + e fa è io come lo faccio l'euro €
Niente paura bro, ALTGR+5 (o Option+5 su macOS) fa €

Se avete altri dubbi, c'è questa immagine epica con tutti i keymap
![Keymaps](https://i.imgur.com/jJ0HwuL.png)

# Installazione su Windows
1. Scaricate [l'ultima release](https://github.com/Sclafus/us_keyboard_with_italian_letters/releases/latest)
2. Decomprimete l'archivio ed eseguite `setup.exe`
3. Aprite le impostazioni di Windows, andate su Data/Ora e Lingua > Lingua
4. Scorrete fino a lingue preferite, cliccate sulla lingua che state utilizzando e poi premete "Opzioni"
5. Nella sezione Tastiere, premete "Aggiungi tastiera" e selezionate `Italiano (US Keyboard with Italian Letters)`
6. Eliminate la vecchia tastiera, cliccandoci sopra e poi premendo Rimuovi

# Installazione su macOS
1. Scaricate il file `Italian (US keyboard with Italian Letters).keylayout` dalla repository (oppure [dall'ultima release](https://github.com/Sclafus/us_keyboard_with_italian_letters/releases/latest))
2. Copiate il file nella cartella `~/Library/Keyboard Layouts/`. Se la cartella non esiste, createla. Da terminale:
   ```bash
   mkdir -p ~/Library/Keyboard\ Layouts
   cp "Italian (US keyboard with Italian Letters).keylayout" ~/Library/Keyboard\ Layouts/
   ```
3. Fate il logout e il login (oppure riavviate il Mac (consigliabile))
4. Aprite Impostazioni di Sistema > Tastiera > Sorgenti di input > Modifica
5. Premete il `+` in basso a sinistra, scorrete fino alla sezione "Altre" e selezionate `Italian (US keyboard with Italian Letters)`
6. Eliminate la vecchia tastiera selezionandola e premendo il `-`
7. Dalla barra dei menu in alto a destra, selezionate il nuovo layout

> **Nota:** su macOS, il tasto **Option (⌥)** sostituisce **ALTGR**. Il tasto **Command (⌘)** conserva tutte le scorciatoie di sistema (⌘C, ⌘V, ⌘Z, ecc.).

# Compilazione manuale (Windows)
Non dovreste mai fidarvi degli eseguibili su internet, anche se sono su GitHub.
Per compilare questo layout:
1. Clonate la repository
2. Scaricate e installate [Microsoft Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134)
3. Aprite Layout Creator, premete su File > Load Source File
4. Scegliete il file `.klc` della repository
5. Andate su Project > Build DLL and Setup Package
6. Aprite la cartella creata e avrete il vostro `setup.exe`, potete seguire il [resto dell'installazione](#installazione-su-windows) saltando il primo passaggio