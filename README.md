# Punto Rosso

Lettore per la lettura veloce (RSVP): incolli un testo o carichi un PDF, il sito riconosce i titoli delle sezioni e mostra una parola alla volta, con la lettera di fissazione in rosso, alla velocità che scegli.

Tutto il sito è il file `index.html`. Non serve nessun server: il testo e i PDF vengono elaborati nel browser di chi lo usa e non lasciano il suo computer.

## Dove cambiare le cose in `index.html`

- **Colori e font**: blocco `:root` all'inizio dello `<style>`.
- **Riconoscimento dei titoli nel testo incollato**: sezione `1. Testo -> sezioni` (funzione `parseText`).
- **Tempo a schermo di ogni parola**: sezione `2. Tempi` (funzione `weight`).
- **Lettura dei PDF**: sezione `5. PDF -> testo con titoli` (funzione `pdfToText`).

Ogni modifica salvata su GitHub viene pubblicata da Vercel in automatico.
