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

## Sådan fungerer koden:
Hver vores (/pages) side består af sit eget indhold af html og css, samt med anvendelse af fælles komponenter for at skabe et bedre overblik og genbrug. Dette er også med til at sikrer en ensartet struktur på tværs af hele sitet.

Derudover anvendes en global.css der indeholder fælles styling, som går igen på tværs af alle sider:

global.css indeholder fælles styling, som går igen på tværs af alle sider:

- Fonts
- Reset (fjerner browserens standard styles)
- Farve variable

## Branches og hvordan de bruges:

Hver gang vi hver især starter på et nyt element i koden oprettes en branch fra Main. Sammen med vores individuelle opsætning gør det det muligt at samarbejde om en kode uden at forstyrre hinandens arbejde og på den måde undgår vi merge conflicts.


## gruppemedlemmer
- Nynne
- Louise
- Ea
- Alex




Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
