---
title: Generel
lang: da_DK
sidebarDepth: 2
---

# Wiki :de: <Badge :text="'LSSM V.' + ($themeConfig.variables.versions.stable || 4)"/>

*Aktuelle versioner:*
> Stable: <i>{{ $themeConfig.variables.versions.stable }}</i> (noch nicht veröffentlicht)
> 
> Beta: <i>{{ $themeConfig.variables.versions.beta }}</i>

<a :href="$themeConfig.variables.discord" target="_blank" style="float: right;"><img src="https://discord.com/api/guilds/254167535446917120/embed.png?style=banner1" alt="Unser Discord-Server: United Dispatch" data-prevent-zooming></a>

## Om LSSM

LSS-MANAGER V.4 er en udvidelse til [Leitstellenspiel.de] (https://www.leitstellenspiel.de) og dens andre sprogversioner.
Med denne udvidelse tilføjes en app-butik til spillet, som tillader installation af plugins. Alle funktioner har en modulær struktur - du kan bestemme, hvad der skal aktiveres indtil den sidste komponent.
Plugins die nicht aktiviert sind, werden auch nicht geladen - das macht die Verwaltung natürlich sehr einfach und sorgt für eine bessere Performance.


## installation :inbox_tray:
Ved at bruge LSSM accepterer du, at vi indsamler metadata. Du kan finde flere oplysninger om dette under [Metadata] (metadata.md)

En tabel med hvilke browsere LSSM er kompatibel kan findes i vores [FAQ] (faq.md # i-hvilke-browsere-gør-det-lss-manager arbejde)

::: tip Brug LSSM på din mobiltelefon
Vi understøtter ikke officielt en mobilversion. Firefox-browseren giver dog også mulighed for at bruge tilføjelsesprogrammer i sin mobile version. Vi garanterer dog ikke et attraktivt design eller fuld funktionalitet for mobile browsere.
Officiel support af mobilbrowsere er i øjeblikket ** ikke ** planlagt.
:::

### Trin 1: Tampermonkey
Hvis du endnu ikke har installeret Tampermonkey i din browser, skal du stadig gøre dette. Her er en oversigt over browser-links:

Browser| link
-------|----
Chrome | [Download](https://chrome.google.com/webstore/detail/dhdgffkkebhmkfjojejmpbldmpobfkfo)
Firefox| [Download](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
Safari | [Download](https://safari.tampermonkey.net/tampermonkey.safariextz)
Opera  | [Download](https://addons.opera.com/en/extensions/details/tampermonkey-beta/)

For andre browsere kan Tampermonkey downloades fra [tampermonkey.net] (https://www.tampermonkey.net/).

::: warning
Bemærk, at vi ikke officielt understøtter ældre browsere, mobilbrowsere og Microsoft Edge eller Internet Explorer. Support til disse browsere er hverken garanteret eller sandsynlig.
:::

### Trin 2: Brugerskript
Hvis Tampermonkey er blevet installeret i din browser, kan du enten <a :href="$themeConfig.variables.server + 'lssm-v4.user.js'" target="_blank">hier</a>eller opret et nyt bruger script med følgende indhold:

<<< ./dist/static/lssm-v4.user.js

### Trin 3: Aktivér
LSSM-indikatoren er LSSM-logoet eller (hvis indstillet i overensstemmelse hermed i [Indstillinger] (indstillinger.md # label-i stedet-ikon-i-menu)) en grøn tekst `LSSM V.4`.
Hvis du er i kontrolcenter-spillet, men ikke kan se denne indikator i øverste højre hjørne, skal du klikke på ikonet Tampermonkey i din browser og kontrollere, om kontakten til LSS-managerscript er indstillet til 'til'.

Hvis du har problemer, kan du altid kontakte [Support] (support.md).
