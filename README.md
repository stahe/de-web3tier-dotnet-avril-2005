# Erstellung einer dreistufigen Webanwendung mit Spring.NET und VB.NET

➡️ Verwandter Kurs:  
[Erstellung einer dreistufigen Webanwendung mit Spring.NET und VB.NET](https://stahe.github.io/de-web3tier-dotnet-avril-2005/)

---

## Einleitung

Dieses Dokument erklärt, wie man eine **dreistufige Webanwendung** mit **VB.NET**, **ASP.NET** und **Spring.NET** entwickelt.  

Ziel ist es, zu zeigen, wie man eine Anwendung strukturiert, indem man folgende Komponenten klar voneinander trennt:
- die Benutzeroberfläche
- die Geschäftslogik
- den Datenzugriff
Das **Spring.NET**-Framework wird verwendet, um die Komponenten der Anwendung nach dem Prinzip **IoC (Inversion of Control)** zu konfigurieren und zusammenzusetzen.

Dieser Ansatz ermöglicht es insbesondere, die Implementierung einer Schicht zu ändern, ohne andere Teile der Anwendung zu beeinflussen. 

---

## Ziele des Tutorials

Die Hauptziele dieses Dokuments sind:

- das Erstellen einer **dreischichtigen Webanwendung**:
  - Benutzeroberfläche
  - Geschäftsschicht
  - Datenzugriffsschicht
- die Konfiguration der Anwendung mit **Spring IoC**
- die Erstellung **mehrerer Versionen der Anwendung** durch Änderung der Implementierung einer oder mehrerer Schichten, um die Flexibilität der Architektur zu veranschaulichen. 

---

## Verwendete Tools

Das Tutorial nutzt die folgenden Tools:

- **Visual Studio .NET** — Entwicklungsumgebung
- **Cassini** — Webserver zur Ausführung der Anwendung
- **NUnit** — Framework für Unit-Tests
- **Spring.NET** — Konfiguration und Integration der verschiedenen Schichten der Webanwendung

---

## Niveau des Dokuments

Dieses Dokument richtet sich an ein Publikum mit **mittlerem bis fortgeschrittenem** Niveau. Zum Verständnis sind fundierte Kenntnisse verschiedener Konzepte im Zusammenhang mit .NET und der Webentwicklung erforderlich. 

---

## Empfohlene Voraussetzungen

Um diesem Tutorial effektiv folgen zu können, sollten Sie mit folgenden Themen vertraut sein:

- der **Sprache VB.NET**
- **der Webentwicklung mit ASP.NET**
- dem Prinzip **IoC (Inversion of Control)**
- den Grundlagen des Frameworks **Spring.NET** 

---

## Empfohlene Ressourcen

Die folgenden Ressourcen können hilfreich sein, um die Voraussetzungen zu erwerben:

- *Einführung in VB.NET anhand von Beispielen*
- *Webentwicklung mit ASP.NET 1.1*
- *Spring IoC für .NET*
- Offizielle Dokumentation zu **Spring.NET**

---

## Kontext und didaktischer Ansatz

Dieses Tutorial orientiert sich an einem ähnlichen Dokument, das im Java-Ökosystem erstellt wurde:

**3-Schichten-Architekturen und MVC-Architekturen mit Struts, Spring und Java**

Das Ziel ist es, zu zeigen, dass:

- die **Java (J2EE)**- und **.NET**-Architekturen auf sehr ähnlichen Prinzipien basieren;
- die in einer Umgebung erworbenen Kenntnisse **in der anderen wiederverwendet** werden können.  
 
--- 
 
## Vorgestellte Architektur 
 
Die entwickelte Anwendung folgt einer **dreistufigen MVC-Architektur**: 
 
Serge Tahé, April 2005