# &#128214;Help Viewer přehled

<!-- @print-keep-icons -->
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
  - &#x1F50E; Hledání slov v textu kapitol  
    *(viditelné jen pokud jej definoval autor nápovědy nebo je aktivní funkcionalita indexace)*

  Tyto položky jsou zobrazeny jako rozbalovací strom s uzly, na které lze kliknout. Kliknutím na položku se rozbalí její dílčí část nebo se otevře vybraná kapitola.  
  &#x1F4C7; a &#x1F50E; mají nahoře pole pro zadání fráze, kterou chcete vyhledávat.  
  Napište frázi a stiskněte **Enter**, abyste zahájili hledání.  
  Kliknutím na **Esc** pole vymažete a opustíte.

  - &#x1F3E1; Přejít na hlavní stránku nápovědy (README.md)

### Nastavení prohlížeče

  - 🌐 Výběr jazyka prostředí
  - 🕘 Najít jinou verzi nápovědy (je potřeba být připojen k Internetu)
  - &#127912; Nastavit schéma barev  
    *(barevné, stupně šedi, bílá a černá, černá a bílá, sepie)*
  - 📚 Zobrazit všechny kapitoly jako jeden dokument  
    *(po výběru zalomení stránek a způsobu tisku Unicode ikon v textu stačí podruhé kliknout na tlačítko a zobrazí se výsledek)*  
    *(do výstupu se zahrnují pouze kapitoly zobrazené ve stromu témat, domovská stránka nápovědy, kapitoly, na které je v textu odkazováno)*
  - ✏️ Poznámky  
    *Umožňuje přidávat, spravovat a přepínat zobrazení (👁️) nebo skrytí (🙈) uživatelských poznámek. Poznámky lze odstranit jednoduchým vymazáním jejich obsahu. Ty, které jsou zobrazené na obrazovce, se automaticky zahrnují i do tisku. Zobrazují se pouze při procházení jednotlivých kapitol. Poznámky se ukládají pouze do Vašeho prostředí a nikdo jiný k nim nemá přístup. Pokud ale přepnete na jinou jazykovou nebo novější verzi stejného souboru nápovědy, zobrazí se v ní vaše poznámky také.*
  - &#8596; Přesunout levý panel na druhou stranu (nebo zpět)
  - &#x1F532; Přepnout full screen režim
  - 📽 Prezentační režim  
    *(Přepnout full screen režim (🔲), klávesy ⬅, ⬆, ➡, ⬇ slouží k přechodu mezi kapitolami/snímky)*
  - 🌈 Vybrat styl  
    *(z rozbalovacího seznamu můžete vybrat jiný styl aplikace)*
  - &#x274C;&#xFE0E; Schovat levý panel

## Pravý panel

Pravý panel zobrazuje hlavní část aplikace:

- Obsah vybrané kapitoly
- Nadpis kapitoly v horním panelu
- Tlačítka:

  - &#x2630; Zobrazit levý panel  
    *(pokud je skrytý)*
  - 🖨️ Vytisknout kapitolu
  - &#x2B05; Přejít k předchozí kapitole
  - &#x2B06; Přejít na nadřízenou kapitolu
  - &#x27A1; Přejít k následující kapitole
  - 📝 Editovat v repozitáři
  - 📥 Export otevřené kapitoly nebo všech kapitol
  
## Proč část prvků chybí?

Může to být z několika důvodů:

| Chybějící prvek | Proč? |
|---|---|
| &#x1F4D6; / &#x1F4C7; | Autor nápovědy nedefinoval potřebná data |
| 🔎 | Autor nápovědy nedefinoval potřebná data, funkce indexace je vypnutá nebo proces indexace nebyl zatím dokončen |
| &#x1F516; | Kapitola nemá podkapitoly |
| &#x2630; | Levý panel je viditelný |
| Levý panel | Schoval jste levý panel, klikněte na horním panelu na tlačítko ☰ a panel se znovu zobrazí |
| 🕘 | Nápověda nemá vazbu na veřejný online repozitář  (např. není k dispozici připojení k internetu) |
| 📥 Export | Správce systému z aplikace odebral celou funkci nebo jednotlivé exportní formáty |

Funkce 📥 Vlastní balíček umožňuje upravit většinu funkcionality. Pokud byla při stažení aplikace použita, některé funkce mohou být nedostupné.

## Data nastavení

Aplikace ukládá část Vaší konfigurace do **local storage**:

| Klíč | Popis |
|---|---|
| colorTheme | Schéma barev (&#127912;) |
| sidebarVisible | Viditelnost levého panelu (&#x274C;&#xFE0E; / &#x2630;) |
| language | Vybraný jazyk prostředí (&#x1F310;) |
| keywordListingCount | Počet klíčových slov, která se budou zobrazovat v seznamech &#x1F4C7;, &#x1F50E;. |
| sidebarSide | Strana levého panelu (&#8596; ; 0 = vlevo, 1 = vpravo) |
| printIcons | Režim tisku unicode ikon; 0 = odstranit, 1 = ponechat, 2 = podle konfigurace autora |
| notesVisible | Režim zobrazení uživatelských poznámek; 0 = skryté (🙈), 1 = zobrazené (👁️) |
| skin | Styl aplikace (🌈; prázdné = výchozí) |
| exportDictionaries | U statického exportu (pokud jej aplikace podporuje) 1 = budou exportovány seznamy (📇, 🔎), 0 = seznamy nebudou součástí exportu |

Modul ✏️ Poznámky uchovává svá data v **IndexedDB** úložišti webového prohlížeče (databáze **HelpViewer**).

# Začínáme

## Otevření souboru nápovědy

Přidejte do adresního řádku parametr **?d={cesta}**. 
Pokud toto neuděláte, bude použita výchozí hodnota: **hlp/Help-{jazyk}.zip** a prohlížeč se pokusí načíst data z tohoto souboru.

Cesta může mít tyto formáty, které končí na:

- .zip - čtení zazipovaného souboru
- / - čtení adresáře nebo adresy ze sítě nebo disku

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
| 🌐 Odkaz na poslední verzi | <span id="linkhereI"></span> |

<script>
  insertDownloadLink('linkhereI', '@ (_)');
</script>
