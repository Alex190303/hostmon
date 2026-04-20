# Teknisk dokumentation: Høst Møn

## Om projektet:
Tema 9:
Vi har i dette tema udarbejdet vores egen database som indeholder oplysninger om kunstnerens ID, billede samt dato og tidspunkt. Løsningen er udviklet med Javaskript, CSS og Html.

## Navigationen af vores løsning:
- Forside
- Menu med oversigt over diverse sider
- Vælg en side
- Se hele lineup
- Sorter og filtrer efter alferbetisk navne og/eller optræden kun lørdag eller kun fredag
- Køb din billet
- Udfyld den via. et vidersendt link til billetto.dk
- Yderligere sider om “Praktisk info” eller "Måltidet" hvis brugeren er interesseret i at vide mere om Høst Møn
- Footer med adresse, kontaktinformationer og sociale medier

## Projekt mappe opsætning:

hoestmon/
├── public/
    └── iconer_illustration
│       └── imgs
├── src/
│   └── components/
│       └── ArtistCard.astro
│       └── Menu.astro
│       └── Footer.astro
│   └── layouts/
│       └── Layout.astro
│   └── pages/
│       └── index.astro
│       └── lineup.astro
│       └── maaltidet.astro
│       └── praktiskInfo.astro
│   └── styles/
│       └── global.css
└── package.json

## Filbeskrivelser

### /public:
Indeholder billeder, ikoner og illustrationer der bliver brugt på siden.

### /src:
Er hovedmappen som indeholder:
/components - genanvendelige komponenter, som bruges på tværs af siderne. 
ArtistCard.astro: Viser navn, tid og dato for hver enkel kunstner
Menu.astro: Navigationsmenu med oversigt over de forskellige sider, der genbruges for hver side.
Footer.astro: Footer med generel information og sociale medier der genbruges for hver side.
/layouts
Layout.astro: Overordnet layout (wrapper), der bruges på tværs af alle sider og definerer vores fælles struktur og opsætning af indhold herunder vores menu og footer. 
/pages
index.astro: Forsiden
lineup.astro: Viser linup af kunstnerne via vores database
maaltidet.astro: Information om det nærværende og festlige måltid på festivalen
praktiskInfo.astro: Praktiske information om den nye placering af Høst Møn

### /styles:
/global.css: Fælles design der gør sig gældene for alle sider. 




```sh
npm create astro@latest -- --template minimal
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
