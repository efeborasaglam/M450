C# **Checkliste zur Codeüberprüfung**

## 1. **Code-Duplizierung**
- [x] Gibt es Methoden oder Codeabschnitte, die dupliziert oder sogar dreifach vorkommen?  
- [x] Kann gemeinsamer Code in eigene Methoden oder Klassen extrahiert werden?  

---

## 2. **Methoden und Klassenanalyse**
- [x] Gibt es zu lange Methoden (übermäßig viele Zeilen Code)?  
- [x] Sind Klassen zu groß (z.B. zu viele Verantwortlichkeiten in einer Klasse)?  
- [x] Gibt es zu lange Parameterlisten in Methoden?  

---

## 3. **Code-Smells prüfen**
- [x] **Duplicated Code**: Überall gleichen oder ähnlichen Code identifizieren.  
- [x] **Shotgun Surgery**: Muss man zu viele Dateien ändern, wenn man etwas Kleines anpasst?  
- [x] **Feature Envy**: Verwenden Methoden zu stark Eigenschaften anderer Klassen?  
- [x] **Datenklumpen**: Existieren viele zusammenhängende Variablen (Clumps of Data)?  
- [x] **Primitive Obsession**: Werden anstatt spezifischer Typen zu viele einfache Datentypen (wie `int`, `string`) genutzt?  
- [x] **Spekulative Verallgemeinerung**: Gibt es Code oder Klassen, die nur für "zukünftige" Anforderungen geschrieben wurden?  
- [x] **Magic Numbers**: Wurden "magische Zahlen" durch Konstanten ersetzt?  

---

## 4. **Codierungsrichtlinien**
- [x] **Namenskonventionen**: Wurden klare und konsistente Namen für Variablen, Methoden und Klassen verwendet?  
- [x] **Formatierung**: Ist der Code sauber formatiert (Einrückungen, Zeilenumbrüche)?  
- [x] **Kommentare**: Gibt es unnötige oder fehlende Kommentare?  
- [x] **Fehlerbehandlung**: Wird Ausnahmen (Exceptions) ordnungsgemäß behandelt?  

---

## 5. **Clean Code Prinzipien**
- [x] **DRY** (Don’t Repeat Yourself): Kommt der gleiche Code mehrfach vor?  
- [x] **KISS** (Keep It Simple, Stupid): Ist der Code so einfach wie möglich gehalten?  
- [x] **YAGNI** (You Aren’t Gonna Need It): Wurde überflüssiger Code vermieden?  
- [x] **Lesbarkeit**: Ist der Code gut lesbar und verständlich?

---

## 6. **SOLID-Prinzipien**
- [x] **SRP** (Single Responsibility Principle): Hat jede Klasse nur **eine einzige Verantwortung**?  
- [x] **OCP** (Open/Closed Principle): Kann Code erweitert werden, ohne bestehenden Code zu ändern?  
- [x] **LSP** (Liskov Substitution Principle): Können Subklassen anstelle der Basisklasse verwendet werden?  
- [x] **ISP** (Interface Segregation Principle): Sind Schnittstellen nicht zu groß und aufgeteilt?  
- [x] **DIP** (Dependency Inversion Principle): Werden Abhängigkeiten über abstrakte Klassen oder Schnittstellen gesteuert?  

---

## 7. **Testbarkeit und Qualitätssicherung**
- [ ] Wurden **Unit Tests** ausreichend implementiert?  
- [ ] **Code Coverage**: Wie hoch ist die Testabdeckung (z.B. 80% oder mehr)?  
- [ ] Sind Tests **unabhängig** voneinander ausführbar?  
- [ ] Gibt es Integrationstests oder andere automatisierte Testverfahren?  

---

### **Bonus: Tools zur Unterstützung**
Um diese Punkte in einer **C#-Applikation** zu prüfen, kannst du folgende Werkzeuge nutzen:  
- **ReSharper** oder **Rider** für Codeanalyse und Refaktorierung  
- **NDepend** zur Codequalität und Regelprüfung (inklusive Code Coverage)  
- **SonarQube** für statische Codeanalyse und Überprüfung der Code-Smells  
- **MSTest, NUnit oder xUnit** für automatisierte Tests  

---