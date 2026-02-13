---
title: Markdown
categories: ["tutorials"]
tags: ["markdown", "tutorial"]
date: 2026-02-04
draft: false
showauthor: true
featureimage: "images/posts/features/markdown-logo.png"
authors:
  - jon-bertelsen
---

## Hvad er Markdown? (kort fortalt)

Markdown er et **letvægts tekstformat**, hvor du skriver helt almindelig tekst + nogle få simple tegn for at få **struktur og formatering**.

Tænk:

> *“plain text som kan blive til flot HTML automatisk”*

Du skriver fx:

```
# Overskrift
**fed tekst**
- liste
```

![Markdown logo](images/logos/markdown-logo.png)
{.fourth-right}

… og det bliver til pænt formatteret indhold på websites, GitHub, Obsidian, README-filer, dokumentation osv.

Det er derfor mega populært blandt udviklere 👇

* README.md på GitHub
* dokumentation
* noter i Obsidian
* statiske sites (Hugo, Astro, Jekyll – som du jo bruger 😉)
* undervisningsmateriale

---

# Mini-tutorial til datamatikerstuderende

Lad os tage det hands-on og praktisk.

Forestil dig du laver:

```
README.md
eller
noter.md
```

---

## 1. Overskrifter

```
# H1
## H2
### H3
```

Bliver til:

# H1

## H2

### H3

💡 Brug dem som i HTML: én H1 pr. side.

---

## 2. Tekstformatering

```
**fed**
*kursiv*
~~overstreget~~
`kode`
```

Resultat:

* **fed**
* *kursiv*
* ~~overstreget~~
* `kode`

💡 `backticks` er guld til kode og variabler.

---

## 3. Lister (meget brugt!)

### Punktliste

```
- Java
- SQL
- Docker
```

* Java
* SQL
* Docker

### Nummereret

```
1. Installer Java
2. Kør Maven
3. Start app
```

1. Installer Java
2. Kør Maven
3. Start app

---

## 4. Links

```
[Google](https://google.com)
```

👉 [Google](https://google.com)

---

## 5. Billeder

```
![alt tekst](image.png)
```

💡 Bruges meget i README’er.

![Javalin logo](images/logos/javalin-logo.png)
{.fourth-left}

<div class="clear"></div>

---

## 6. Kodeblokke (super vigtig for jer)

### Inline

```
List<String>
```

### Multilinje

<pre>
```java
List<String> names = List.of("Jon", "Ada", "Linus");

names.stream()
     .filter(n -> n.startsWith("J"))
     .forEach(System.out::println);
```
</pre>

Bliver:

```java
List<String> names = List.of("Jon", "Ada", "Linus");

names.stream()
     .filter(n -> n.startsWith("J"))
     .forEach(System.out::println);
```

💡 Skriv sproget → syntax highlighting (java, js, sql, bash osv.)

---

## 7. Tabeller (god til data/øvelser)

```
| Navn | Sprog | Niveau |
|------|--------|----------|
| Anna | Java   | 7/10 |
| Bo   | SQL    | 9/10 |
```

| Navn | Sprog | Niveau |
| ---- | ----- | ------ |
| Anna | Java  | 7/10   |
| Bo   | SQL   | 9/10   |

Perfekt til:

* karakterer
* commits
* opgaver
* sprint boards

---

## 8. Citater

```
> Husk at committe ofte
```

> Husk at committe ofte

---

## 9. Checkbokse (mega nice til todo)

```
- [x] Lav database
- [ ] Skriv tests
- [ ] Deploy
```

* [x] Lav database
* [ ] Skriv tests
* [ ] Deploy

Virker i GitHub + Obsidian + mange editors.

---

# Mini øvelse (til studerende)

Lad dem lave:

## Opgave

Lav en `README.md` til jeres projekt med:

* Projekttitel
* Kort beskrivelse
* Teknologier
* Installation steps
* Kodeeksempel
* Todo liste

### Skabelon

````md
# Mit Projekt

## Beskrivelse
Kort forklaring på hvad appen gør.

## Teknologier
- Java 17
- Javalin
- PostgreSQL
- Docker

## Installation
```bash
mvn clean install
docker compose up
````

## Eksempel kode

```java
app.get("/hello", ctx -> ctx.result("Hej verden"));
```

## TODO

* [ ] Tests
* [ ] Swagger
* [ ] Deploy

```

---

# Hvornår skal man bruge Markdown?

Brug det når:

✅ dokumentation  
✅ noter  
✅ GitHub  
✅ undervisningsmateriale  
✅ statiske websites (Hugo/Geekdoc/Next content)  
❌ avanceret layout → brug HTML/CSS

