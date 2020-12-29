---
title: FAQ ❓
lang: da_DK
sidebarDepth: 3
---

# FAQ ❓

### Hvad koster LSS-manager?
LSS Manager er et gratis tilbud - vi har heller ikke planer om at ændre det.
Selvom det bestemt tilføjer værdi, er der ingen moms på dette produkt:wink:

::: warning donere
Der er et par gode brugere, der gerne vil donere penge til os. Men: LSS Manager er og forbliver gratis. Vi accepterer heller ikke nogen donationer til dette projekt.

Der er flere grunde til dette:

* Dette projekt er videreudviklet på frivillig basis i de involverede udviklers fritid
* En abonnementsvariant, der ligner præmien i spillet, ville lægge for meget pres på os personligt for at fortsætte programmeringen ud over vores ønske.
* Af juridiske årsager kan vi ikke acceptere donationer:
    * Hvis vi skulle starte en virksomhed for LSS-lederen, så vi kunne modtage donationer, ville det ikke have nogen fremtid, da en virksomhed ikke kan være en virksomhed uden at bruge penge.
    * Hvis vi lader de servere, der i øjeblikket er ansvarlige for LSS-manager i baggrunden, køre gennem et firma, spiser de straks indkomsten.

Derfor giver det ingen mening for os udover ideen om frivillighed at tage penge til LSS-lederen.

### Hvordan kan jeg bidrage til LSS Manager?
Den "normale" bruger kan [Fehler melden][error] eller [Vorschläge einreichen][suggestions]

Wir gestalten derzeit einen Styleguide für Entwickler, damit auch diese einfach eigene Plugins dem LSSM hinzufügen können. Zudem haben wir versucht, die Code-Struktur übersichtlich und verständlich zu halten. Das Hinzufügen eines Plugins bedeuted jedoch keinenfalls eine Aufnahme in das Team.

### Wie melde ich Fehler?
Bitte schaue dir unsere Seite [Fehler melden][error] an.

### Wo bekomme ich Hilfe?
Über unseren Support. Nähere Infos dazu gibt es [hier][support].

### Wie kann ich Vorschläge einreichen?
Auf der Seite [Vorschläge][suggestions] haben wir dir Informationen darüber zusammengestellt.

### In welchen Browsern funktioniert der LSS-Manager?
Hier werden nur Desktop Browser aufgelistet, da mobile Browser nicht offiziell unterstützt werden.
Diese Tabelle ist noch nicht umbedingt korrekt und wird bei neuen Informationen aktualisiert!

Da wir durchgängig neueste Coding-Standards einhalten möchten, ist ein moderner und aktueller Browser notwendig und empfehlenswert - schon allein aus Sicherheitsgründen, auch außerhalb des Spiels.

::: warning Kompatibilität
Eine hier aufgelistete Kompatibilität gewährleistet keine Funktionalität. Dies sind nur Informationen, die von Drittanbietern zusammengetragen und ausgewertet wurden.
:::

<table>
    <thead>
        <tr>
            <th>Browser</th>
            <th>mind. version</th>
            <th>Download</th>
        </tr>
    </thead>
    <tbody>
        <tr v-for="({supported, download}, browser) in $themeConfig.variables.browsers">
            <td>{{ browser.replace(/^./, $1 => $1.toUpperCase()) }}</td>
            <td>{{ supported }}</td>
            <td><a :href="download" target="_blank">Download</a></td>
        </tr>
    </tbody>
</table>

::: danger Internet Explorer und Microsoft Edge
Diese beiden Browser kann man als "Problemkinder" eines modernen Web-Entwicklers beschreiben. Es gibt einige Funktionen, die in ihnen nicht funktionieren, oder zusätzlichen Code benötigen.

Wir sehen es nicht ein, dies überall zu machen und unterstützen diese beiden Browser offiziell **nicht**.
:::

### Ich möchte mein Setup an Freunde weitergeben oder es an mehreren Geräten nutzen. Geht das?
Aktuell geht das nicht, wir arbeiten aber daran, das einzubauen.

### Gibt es eine Möglichkeit, Einstellungen Account-gebunden zu speichern, um sie an einem anderen Gerät nicht importieren zu müssen?
Derzeit bieten wir das nicht an, eine Implementierung dieses Features ist aber geplant.

### Wo so seh ich ob die LSSM-Server grad online sind? 
Am besten hier: [https://status.lss-manager.de/](https://status.lss-manager.de/)
Oder im Uptime-Channel auf unserem <a :href="$themeConfig.variables.discord" target="_blank">Discord</a> 

[support]: support.md
[error]: error_report.md
[suggestions]: suggestions.md
