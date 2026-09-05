# Uppgift: Individuell uppgift i databashantering

## Beskrivning

Uppgiften går ut på att du individuellt arbetar med din tilldelade variant och skriver en rapport som behandlar de moment som ingår i uppgiften.

## Inför uppgiften

- Sätt dig in i vad [Markdown][md] är, särskilt hur man skriver rubriker med `#`, hur man gör punktlistor och numrerade listor, samt hur man skriver "inline-kod" och kodblock. Det är enklare än det låter!

- Bekanta dig med [Mermaid][mm], särskilt hur det används för att skapa t.ex. Entity Relationship Diagram (ERD), vilket kan vara till stor nytta i kursen.

- Om båda ovanstående punkter tillsammans tar mer än en halvtimme, är risken hög att du är mer noggrann än vad som krävs.

## Krav

### Innehåll

- Placera följande mall, ifylld, direkt under huvudrubriken. Ersätt A–E med bokstaven för den uppgiftsvariant du tilldelats, och G/VG med det betyg du siktar på. Du kan börja med G och byta till VG vid behov.

  ```plaintext
  Uppgiftsvariant: A–E
  Betyg: G/VG
  ```

- Använd exakt en huvudrubrik och därefter underrubriker. Använd punktlistor eller numrerade listor vid behov, samt kod i text och kodblock. Kom ihåg att börja meningar med stor bokstav och undvik alltför långa rubriker. Dela in texten i stycken för att undvika "wall of text".

### Rapportens teknik

- Skriv dokumentet som en vanlig textfil i [Markdown][md]-format, utan HTML.

  - Placera eventuella bilder i katalogen `img/` och länka dem så att de visas korrekt när Markdown-filen renderas. Använd “Markdown Preview” i VSCode eller visa filen `uppgift.md` på GitHub efter att du gjort en push.

  - Det är ännu bättre att undvika bildfiler och i stället bädda in [Mermaid][mm]-diagram direkt i Markdown-texten.

- Använd rubriker med `#`, `##`, `###` och punktlistor med `-`.

- Använd "inline-kod" eller kodblock för allt som räknas som kod, till exempel terminalkommandon och SQL.

  - *Inline-kod* används i löpande text, som till exempel hur `SELECT * FROM Users` används för att lista alla kolumner för alla rader i `Users`.
  - *Kodblock* används för flera kodrader i rad. Exempel:

  ```sql
  SELECT
    *
  FROM Employee
  WHERE role = "devops"
  ```

  - Märk alltid kodblock med ett språknamn. SQL-exempel ska använda ` ```sql `, och övriga block ska använda ett passande språk (eller `plaintext` om inget bättre finns).

- Se till att verktyget Markdownlint inte visar några fel för din `rapport.md`. Använd den medföljande konfigurationsfilen för verktyget. Kontrollera fliken “Problems” i din editor. Vid inlämning ska bygget markeras med en grön bock, vilket visar att Markdownlint inte har påtalat några problem.

## Inlämningsinstruktioner

Läs dokumentet [Studentguide till GitHub Classroom][sgc].

### Filer

Alla filer utom de som matchar mönstren nedan ignoreras i `.gitignore` för att hålla inlämningen prydlig, fokuserad och lätt att förstå.

**Obligatoriska filer:**

| Filnamn      | Beskrivning        |
| ------------ | ------------------ |
| `rapport.md` | Själva dokumentet. |

**Valfria filer:**

| Filnamn | Beskrivning                                  |
| ------- | -------------------------------------------- |
| `img/*` | Eventuella bildfiler som länkas i rapporten. |

[md]: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github
[mm]: https://mermaid.js.org
[sgc]: https://github.com/nackc8/kursmaterial/blob/main/shared/studentguide-till-github-classroom.md
