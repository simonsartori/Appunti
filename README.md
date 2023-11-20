
LINUX
Linux è stato scritto da più di 10000 utenti lungo circa 20 milioni righe di codici

66% of the world server 100% of top 50 supercomputer

The Linux file system used to resemble an unorganised town where individuals construct their houses

wherever they pleased. However, in 1994, the Filesystem Hierarchy Standard (FHS) was introduced to bring

order to the Linux file system.

By implementing a standard like the FHS, software can ensure a consistent layout across various Linux

distributions. Nonetheless, not all Linux distributions strictly adhere to this standard. They often incorporate

their own unique elements or cater to specific requirements.

To become proficient in this standard, you can begin by exploring. Utilise commands such as "cd" for

navigation and "ls" for listing directory contents. Imagine the file system as a tree, starting from the root (/).

With time, it will become second nature to you, transforming you into a skilled Linux administrator.

Some fundamental things to know
Kernel --> brain of the Linux operating system controls the Hardware and make interract whit applications.

Distribution --> collection of programs combined whit the kernel to make a Linux based operating system.

Filesysyem --> Method for storing and organizing files.

Command line --> interface for typing command on top of the operating system.

Shell --> command line intrepreter.

Directory --> is a location for storing files.

REPL = Read–Eval–Print Loop è il modo di funzionamento della maggior parte delle CLI e' in breve e' un ambiente di programmazione che accetta un input lo valuta e restituisce il risultato.

CLI = command line interface.

Prompt = è un programma che emula il campo di input in una schermata dell'interfaccia utente basata su testo con l'interfaccia utente grafica.
LINUX COMANDS
General structure
command [-flag(s)] [-option(s) [value]] [argument(s)]

flag --> modify the operation of commands and are sommetimes called options
options --> help to define how a commands should behave(comportarsi)
argument --> arguments tell a commands what objects to operate on
Commands



man = manual page (è un manuale per un comando)

tree =  fa vedere tutta la struttura del file suystem a albero

dir = elenca il contenuto della directory

ls = elenca informazioni sul file o sulla directory

mkdir = creare una nuova directory

groupadd = creare un nuovo gruppo

rm = rimuovere un file o directory

cp = copiare file o directory

mv = muovere o rinominare il file o directory

chmod = cambiare i permessi sul file o directory 

chown = modificare la proprietà di un file o di una directory

grep = global regular expression print --> search for a pattern in files

find = Search for files and directories

tar = manipulate tarball archive files

vi = Edit files using text editors
nano - una cosa molto simile e meno complessa

cat = display the content of files

top = Display processes and resource usage

ps = Display processes information

kill = Terminate a process by sending a signal

du = Estimate file space usage

ifconfig = Configure network interfaces

ping = Test network connectivity between hosts

set =  fa vedere i nomi e i valori di tutte le variabili e funzioni

env = Scrive una lista di variabili d'ambiente o far runnare altre robe

type = dice che comando è e dove si trova

switch = dice dove si trova

ps f = fa vedere i processi

less = per leggere il contenuto di file di testo

su = permette di avviare una shell testuale assumendo l'identità di un altro utente del sistema

exit = termina il processo
Variabili d’ambiente importanti sfruttati dalla Shell e dalla Bash
$SHELL fa vedere la shall attuale
$HOME dice quale la home directory
La shell tiene traccia dei comandi che eseguiti per default
HISTSIZE = ti dice quanto spazio hai

history = è la storia dei comandi usati
Ogni processo in esecuzione attiva 3 file
stdin = Standard input si aspetta quello che scrivete
stdout = Standard output scrive sul terminale (quello che viene mostrato sullo schermo)
stderr = Standard error butta fuori sia messaggi usciti sia quelle di errore

Tutti questi tre file corrispondono al terminale.
Pipe = | = serve per muovere un data tra due comandi l'output di uno fa da input per l'altro

grep = global regular expression print cercare testo o frasi in un file

exit status = e’ un codice che i programmi possano comunicare alla loro uscita per sapere come sono usciti --> Lo stato di uscita 0 indica che il comando ha avuto esito positivo senza errori invece da 1 a 255 il comando no e' andato a buon fine. echo $? = exit status del punto precedente Alcuni prompt segnalano questa cosa direttamente nella prompt

"<" ">" and "<<" ">>"
"<"  and "<<" sono input redirezioni
“>” and “>>” sono uotput redirezioni
Differenza tra > >>:
    > ">"
        sovrascrive un file esistente o lo crea se non esiste
    > ">>
        appende un file o lo crea se non esiste
(cat) /etc/passwd = un file di sette campi delimitati da due punti contenente informazioni di base sugli utenti

/etc/shadow = un file di nove campi delimitati da due punti contenente le password utente crittografate

/etc/group = un file di quattro campi delimitati da due punti contenente informazioni di base sui gruppi

UID = user id --> numero associato al user

GID = group id --> numero associato al gruppo

La prima lettera indica il tipo di file

Hash → crittografica invertibile, funzione che prende un testo in chiaro di qualsiasi e restituisce un codice una stringa di lunghezza fissa. Qualsiasi stringa al mondo dia sempre un hash diversa che sia innativa.

Se cambio anche un bit del messaggio originale l'hash mi viene totalmente diversa

passwd = era leggibile da tutti e venivano messe le password criptate

Password salvata →  salvato il codice di Hash

Quando si mette la password il sistema mette il testo in chiaro calcola l’Hash e lo confronta
Permessi del file
ls -l --> fa vedere i permessi del file

Prima lettera --> tipologia del file
"-" → File regolare
"d" → directory
"l" → link
permessi delle 3 categorie
Il primo  → user 
secondo  → group
terzo → others 
3 tipi
r --> read = di lettura
w --> wright = di scrittura
x --> execution = di esecizione 
NB il "-" indica la mancanza di permesso
La directory serve per leggere , scrivere e esecuzione di una directory

:: separano la funziona d’ambiente path

Variable
Esistono due tipi di variabili
    Environment variable (variabile d'ambiente) --> vengono ereditate da tutti i processi e le shell del sistema.

    Nella bash ce differenza tra “ e ‘

    "" All’interno dei doppi apici è attiva la sostituzione

    '' All’interno dei singoli apici la sostituzione non è attiva

    (shell)Variables --> si applicano solamente nella shell corrente

    concetto di scope -->  è l'ambito di visibilità di una certa variabile

    Possono contenere solo letteren, numeri e undescore (_)

    Si dichiarano variabile=value  es --> VAR1="cicciogamer" or VAR2=89

    $ per accederci al valore nella variabile (es. $VAR2)

    echo = serve per scrivere lines of string or text del argomento

    export  = rende la variabile della shell in una Environment variable(variabile d'ambiente)

    unset = serve per tirare
