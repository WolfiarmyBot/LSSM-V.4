---
title: ℹ️ General
lang: da_DK
sidebarDepth: 2
---

# ℹ️ Generel information om moduler

På de følgende sider finder du en beskrivelse af alle vores moduler. Vi har gjort vores bedste for at holde dem så forståelige og komplette som muligt. På grund af størrelsen på LSSM er det dog ikke altid let.

Hvis du har forslag til forbedringer, kan du sende dem til os som altid - eller endda bygge dem selv.

:::danger Moduler og indstillinger, der ikke fungerer i Mapkit
Som beskrevet i forklaringen på [Appstore] (appstore.md) er der moduler og indstillinger, som desværre ikke er kompatible med korttypen 'Mapkit'. Disse er disse moduler:
<ul>
    <li v-for="module in $themeConfig.variables.noMapkitModules.de_DE" :key="module.title">
        <router-link :to="module.f">
            {{ module.title }}
        </router-link>
    </li>
</ul>
   Og disse indstillinger:
<ul>
    <li><router-link to="modules/generalExtensions">
        Og disse indstillinger:
        <ul>
            <li><router-link to="modules/generalExtensions#kartensprunge-speichern">
                Gem kortspring
            </router-link></li>
        </ul>
    </router-link></li>
</ul>
:::
