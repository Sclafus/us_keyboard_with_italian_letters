# Perché questo layout è meglio delle alternative per scrivere in italiano?
Non lo è. Personalmente lo trovo più adatto rispetto alle alternative,
ma ciò non implica che sia migliore per qualche ragione oggettiva.

Questo layout è presente nativamente su Linux, è un banale porting.

L'alternativa che viene solitamente proposta è il layout Americano internazionale.

Le motivazioni per cui penso sia superiore per la scrittura in lingua italiana sono:
- Assenza di "dead-keys", che rallentano pesantemente la scrittura
- Tutte le lettere accentate sono nel terzo livello (alt destro).

Per fare le lettere accentate, basterá fare ALT destro + lettera. ALT destro viene anche chiamato ALT GR.

# Ma quindi come si fanno le accentate non ho capito bro
| Combinazione | Risultato |
| ------------ | --------- |
| ALTGR + a | à |
| ALTGR + e | è |
| ALTGR + i | ì |
| ALTGR + o | ò |
| ALTGR + u | ù |
| ALTGR + z | á |
| ALTGR + d | é |
| ALTGR + k | í |
| ALTGR + l | ó |
| ALTGR + j | ú |

Quindi, banalmente, ALTGR + vocale fa la lettera con l'accento grave, mentre premere la lettera esattamente sotto ne fa la versione con l'accento acuto.

## Ok ma se voglio fare l'accentata maiuscola cosa devo fare scusa
Esattamente la stessa combinazione fatta qui sopra, ma tenendo premuto SHIFT oppure inserendo CAPS LOCK.

## Ok bro penso di aver capito ma se ALTGR + e fa è io come lo faccio l'euro €
Niente paura bro, ALT+5 fa €

Se avete altri dubbi, c'è questa immagine epica con tutti i keymap
![Keymaps](https://i.imgur.com/jJ0HwuL.png)

# Installazione
1. Scaricate [l'ultima release](https://github.com/Sclafus/us_keyboard_with_italian_letters/releases/latest)
2. Decomprimete l'archivio ed eseguite `setup.exe`
3. Aprite le impostazioni di Windows, andate su Data/Ora e Lingua > Lingua
4. Scorrete fino a lingue preferite, cliccate sulla lingua che state utilizzando e poi premete "Opzioni"
5. Nella sezione Tastiere, premete "Aggiungi tastiera" e selezionate `Italiano (US Keyboard with Italian Letters)`
6. Eliminate la vecchia tastiera, cliccandoci sopra e poi premendo Rimuovi


# Compilazione manuale
Non dovreste mai fidarvi degli eseguibili su internet, anche se sono su GitHub.
Per compilare questo layout:
1. Clonate la repository
2. Scaricate e installate [Microsoft Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=102134)
3. Aprite Layout Creator, premete su File > Load Source File
4. Scegliete il file `.klc` della repository
5. Andate su Project > Build DLL and Setup Package
6. Aprite la cartella creata e avrete il vostro `setup.exe`, potete seguire il [resto dell'installazione](#installazione) saltando il primo passaggio