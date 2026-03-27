# Hi, I'm Eugen | Systems Architect in TypeScript and Go 🏎️💨

Ich entwickle Software, die schneller ist als die Engines, auf denen sie läuft. Mein Fokus liegt auf **Extreme Performance**, **Zero-Copy-Architekturen** und dem Ausreizen der physikalischen Grenzen von **TypeScript**.

## 🛠️ Die Philosophie: "Mechanical Sympathy"
Ich glaube nicht an "gut genuge" Performance. Ich glaube daran, die zugrunde liegende Engine (V8/JSC) so tief zu verstehen, dass man ihren Overhead umgehen kann. Meine Projekte sind darauf ausgelegt, Garbage Collection (GC) Pausen und Objekt-Overhead zu eliminieren, indem Speicher als rohe, hochperformante Ressource behandelt wird.

> *"JavaScript wurde für Bequemlichkeit entworfen. Ich nutze es für Durchsatz."*

---

## 🚀 Highlight-Projekt: **BumpArena**
**Die ultra-schnelle, Zero-Overhead Memory Arena für Bun & Node.js.**

BumpArena ist ein 1,8 kB Kraftpaket, das neu definiert, wie wir Millionen von Datensätzen in TypeScript verarbeiten. Es umgeht das Standard-JS-Objektmodell, um rohe, deterministische Performance zu erreichen.

* **1,8 kB** Minified (Null Abhängigkeiten).
* **3M+ Records/s** Durchsatz.
* **Zero GC Pressure:** Speicherverwaltung in einem flachen `ArrayBuffer`.
* **Die Ironie:** Ein Tool, das so optimiert ist, dass der einzige verbleibende Flaschenhals die Antriebswelle der Engine selbst ist.

---

## 🧪 In Arbeit: **FlexBuf**
Der logische Nachfolger der Arena. Ein **Zero-Copy JSON-Parser**, der keine Instanzen erzeugt.

* **No String Parsing:** Nutzt `start` und `length` Offsets direkt aus dem Buffer.
* **Fixed-Point Math:** Parsed Zahlen mit Integer-Multiplikations-Tricks, um den `parseFloat`-Overhead zu vermeiden.
* **Das Ziel:** Daten vom Stream zur Logik bewegen mit buchstäblich **null** intermediären Objekten.

---

## 📊 Performance über Hype
Ich bevorzuge eine **1,8 kB** Lösung, die ein Problem dauerhaft löst, gegenüber einem **50 MB** Framework, das es nur versteckt.

| Metrik | Standard TS/JS | Mein Ansatz (Arena/FlexBuf) |
| :--- | :--- | :--- |
| **Speicher** | Aufgebläht durch Objekt-Header | Pure binäre Dichte |
| **Cleanup** | Unvorhersehbare GC-Pausen | O(1) Instant Reset |
| **Speed** | Engine-Limitiert (Logik) | Engine-Bound (Hardware) |

---

## ⚡ Fun Fact
Ich habe eine Woche lang keinen Code geschrieben, weil die Architektur im Kopf reifen musste. Das Ergebnis? Ein Refactoring-Roundtrip, der `alloc` so weit destilliert hat, dass es jetzt die pure Essenz von Geschwindigkeit ist.

## 📫 Connect mit mir
* **Aktuelle Themen:** Low-Level Optimierungen in Bun, Byte-Level Manipulation und SharedArrayBuffers.
* **Frag mich:** Warum deine 10 Millionen Objekte deine App-Latenz töten.

---
*Generated with a touch of irony and peak performance.*
