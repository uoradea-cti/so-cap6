# Sisteme de Operare – Capitolul 6: Mecanismul fork și exec

**1.** Să se scrie un program care să creeze două sau mai multe procese fiu.

**2.** Să se scrie un program C care să creeze două procese fiu și să aștepte terminarea fiecăruia. Procesele fiu se termină unul prin apelul `exit`, iar celălalt printr-un semnal trimis cu funcția `kill` (se alege `SIGQUIT` sau `SIGINT`). Se va include în program și funcția `interpret_stare()` din lucrare.

**3.** Realizați un program interpretor de comenzi care acceptă următoarele instrucțiuni:
- `sort source destination` – sortează conținutul fișierului `source` în fișierul `destination`;
- `search text ext n` – caută acele fișiere cu extensia `ext` care conțin de minim `n` ori șirul de caractere `text`. Când găsește un astfel de fișier, salvează următoarele informații pe linii separate, într-un fișier log: calea absolută a fișierului, data creării fișierului, mărimea fișierului, numărul de apariții a textului căutat.

Când este introdusă o comandă, interpretorul va crea un proces fiu, care va trebui să efectueze comanda.

**4.** Implementați apelurile `execvp` și `execlp` ca subrutine ce folosesc apelurile `execl` și `execv`.

## Compilare și rulare

```bash
cd ex01
gcc -Wall ex01.c -o ex01
./ex01
```
