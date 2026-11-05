# Elf Express Balance Test (Versions A–J)

## What this is
This is a playtest for **Elf Express** with **10 versions, labeled A through J**. Every version is the same game, with different difficulty settings.

## How to open each version
Add `?mix=` and a letter (`A` through `J`) to the end of the `elfexpress.html` link.

For example, locally:
- `http://localhost:8001/elfexpress.html?mix=A`
- `http://localhost:8001/elfexpress.html?mix=B`

The staging link will look the same, just with the staging site address at the start instead of `http://localhost:8001` (for example, `<staging-url>/elfexpress.html?mix=A`).

## How to check you're on the right version
You can check the **Version** badge in the top-left corner, and check how many gifts **Sleigh 1** needs to fill:

| Version | Gifts needed for Sleigh 1 |
| :---: | :---: |
| **A** | 8 |
| **B** | 5 |
| **C** | 6 |
| **D** | 8 |
| **E** | 8 |
| **F** | 6 |
| **G** | 6 |
| **H** | 5 |
| **I** | 8 |
| **J** | 6 |

## How to test
1. **Don't play in order from A to J.** Mix up the order you try them in so earlier games don't bias later ones.
2. **Play on a phone if possible.** If you don't have a phone handy, play on whatever device you have and note your input type.
3. **Play each version at least twice** so you get a real feel for its pace after warming up.
4. **Rate right after each game** in the rating sheet Ania shares while the run is still fresh (you can also use the quick rating buttons between sleighs and download your ratings text file at the end of a run).

---

## For engineers: running locally from this branch
```bash
git fetch origin
git checkout elfexpress-balance-test
npm ci
npm start -- --port=8001
```
Then open `http://localhost:8001/elfexpress.html?mix=A` (or `?mix=B` through `?mix=J`).
