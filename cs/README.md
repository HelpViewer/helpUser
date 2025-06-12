# &#128214;Help Viewer přehled

Aplikace je rozdělena na dvě hlavní oblasti:

## Levý panel

Levý panel umožňuje procházet soubor nápovědy.

Ve spodní části panelu najdete několik tlačítek:

### Navigace v nápovědě

  - &#x1F4D6; Strom témat  
    *(viditelné jen pokud jej definoval autor nápovědy)*
  - &#x1F516; Seznam podkapitol  
    *(viditelné jen pokud má vybraná kapitola podkapitoly)*
  - &#x1F4C7; Seznam klíčových slov  
    *(viditelné jen pokud jej definoval autor nápovědy)*

  Tyto položky jsou zobrazeny jako rozbalovací strom s uzly, na které lze kliknout. Kliknutím na položku se rozbalí její dílčí část nebo se otevře vybraná kapitola.

  - &#x1F3E1; Přejít na hlavní stránku nápovědy (README.md)

### Nastavení prohlížeče

  - &#x1F310; Výběr jazyka prostředí
  - &#127912; Nastavit schéma barev  
    *(barevné, stupně šedi, bílá a černá, černá a bílá)*
  - &#x1F532; Přepnout full screen režim
  - &#x274C;&#xFE0E; Schovat levý panel

## Pravý panel

Pravý panel zobrazuje hlavní část aplikace:

- Obsah vybrané kapitoly
- Nadpis kapitoly v horním panelu
- Tlačítka:

  - &#x2630; Zobrazit levý panel  
    *(pokud je skrytý)*
  - &#x1F4C4; Vytisknout kapitolu
  - &#x2B05; Přejít k předchozí kapitole
  - &#x2B06; Přejít na nadřízenou kapitolu
  - &#x27A1; Přejít k následující kapitole
  
## Proč část prvků chybí?

Může to být z několika důvodů:

| Chybějící prvek | Proč? |
|---|---|
| &#x1F4D6; / &#x1F4C7; | Autor nápovědy nedefinoval potřebná data |
| &#x1F516; | Kapitola nemá podkapitoly |
| &#x2630; | Levý panel je viditelný |
| Levý panel | Schoval jste levý panel, klikněte na horním panelu na tlačítko ☰ a panel se znovu zobrazí |

## Data relace

Aplikace ukládá část Vaší konfigurace do **local storage**:

| Key | Description |
|---|---|
| colorTheme | Schéma barev (&#127912;) |
| sidebarVisible | Viditelnost levého panelu (&#x274C;&#xFE0E; / &#x2630;) |
| language | Vybraný jazyk prostředí (&#x1F310;) |

# Začínáme

## Otevření souboru nápovědy

Přidejte do adresního řádku parametr **?d={cesta}**. Pokud toto neuděláte, bude použita výchozí hodnota: **hlp/Help-{jazyk}.zip** a prohlížeč se pokusí načíst data z tohoto souboru.

## Tipy pro prohlížeč

Moderní webové prohlížeče umí následující funkce:

### 🧭 Navigace v obsahu

| Klávesová zkratka | Akce |
|---|---|
| Tab | Na následující tlačítko / odkaz na stránce |
| SHIFT + Tab | Na předchozí tlačítko / odkaz na stránce |
| ↑ ↓ ← → | Posouvání a pohyb v obsahu (pokud je možné) |
| PageUp / PageDown | Posun o viditelnou stránku výše/níže |

### &#127760; Navigace prohlížeče a akce stránky

| Klávesová zkratka | Akce |
|---|---|
| ALT + ← / → | Zpět a Vpřed v historii procházení |
| CTRL + L | Přejít na adresní řádek |
| CTRL + D | Přidat stránku do záložek |

### &#x1F50D; Zobrazení a zvětšení

| Klávesová zkratka | Akce |
|---|---|
| CTRL + kolečko myši | Přiblížit / Oddálit, Zvětšit / Zmenšit text |
| CTRL + 0 | Nastavit výchozí zvětšení |
| F11 | Přepnout / Ukončit režim celé obrazovky (stránky nebo vnořeného rámce) |
| ESC | Ukončit režim celé obrazovky |
| F3 / CTRL + F | Hledat na stránce |

### &#x1F501; Znovunačtení obsahu

| Klávesová zkratka | Akce |
|---|---|
| CTRL + R / F5 | Obnovit stránku |
| CTRL + SHIFT + R | Obnovit stránku bez použití cache paměti |

### &#x1F4BE; Aplikace a instalace

| Klávesová zkratka | Akce |
|---|---|
| Ikona na adresním řádku (&#x1F4E5;) na pravé straně | Instalovat webovou aplikaci (pokud ji web nabízí) |
