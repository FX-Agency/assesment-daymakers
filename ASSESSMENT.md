# Daymakers Developer Assessment

Met dit assessment willen we inzicht krijgen in je backend- en frontendvaardigheden.
We kijken naar de structuur van je applicatie, de consistentie van je code en de
keuzes die je maakt. Een pixel-perfect ontwerp is niet nodig; een logische,
verzorgde en bruikbare uitwerking wel.

Besteed maximaal **8 uur** aan de opdracht. Stel prioriteiten en beschrijf bij de
oplevering wat je hebt afgerond en wat je met meer tijd zou verbeteren.

## De opdracht

Bouw een kleine eventwebsite waarop een bezoeker een event kan bekijken en zich
met een e-mailadres kan aanmelden.

Gebruik Laravel voor de backend, Inertia.js en React voor de frontend, en
Tailwind CSS en/of (S)CSS voor de styling.

## De eventpagina

Een event bevat:

- Een titel en subtitel.
- Een beschrijving.
- Een start- en einddatum.
- Een locatie.
- Een hero-afbeelding.
- Een unieke slug voor de URL.

De publieke pagina is bereikbaar via `/events/{slug}` en toont deze informatie in
een overzichtelijke layout. Gebruik een hero-sectie met de afbeelding, titel en
subtitel, een sectie met praktische informatie en ruimte voor de beschrijving.
Maak duidelijk hoe de bezoeker zich kan aanmelden.

De pagina moet goed werken op desktop en mobiel. Let op visuele hiërarchie,
spacing, typografie en leesbaarheid. Een onbekende slug geeft een 404-pagina.

## Aanmelden

Houd de aanmelding klein: **één e-mailveld en een aanmeldknop zijn voldoende**.
Je mag dit direct op de eventpagina plaatsen. Een uitgebreid formulier, een
gebruikersaccount of een aparte registratiepagina is niet nodig.

Zorg dat:

- Het e-mailveld verplicht is en server-side wordt gevalideerd.
- Een ontbrekend of ongeldig e-mailadres een duidelijke foutmelding bij het veld geeft.
- Een geldige aanmelding wordt opgeslagen bij het juiste event.
- De bezoeker na een geslaagde aanmelding een duidelijke bevestiging op de pagina ziet.
- Hetzelfde e-mailadres zich niet meerdere keren voor hetzelfde event kan aanmelden.
  Toon in dat geval een begrijpelijke melding.

Geef het veld een zichtbaar label en zorg dat aanmelden ook met het toetsenbord
werkt. Je hoeft geen bevestigingsmail te versturen.

## Technische verwachtingen

- Gebruik migrations voor het datamodel en leg de relatie tussen events en
  aanmeldingen vast.
- Genereer de slug op basis van de eventtitel en houd rekening met unieke URL's.
- Geef eventdata vanuit Laravel via Inertia door aan React.
- Kies een duidelijke componentstructuur en houd je code leesbaar en consistent.
- Voeg enkele gerichte tests toe, bijvoorbeeld voor een geldige aanmelding,
  ongeldige invoer of een onbekende eventslug.

Lever minimaal één voorbeeld-event mee, bij voorkeur via een seeder. Voor de
hero-afbeelding volstaat een lokaal bestand of een afbeeldings-URL die je bij het
event opslaat. Een uploadfunctie, CMS of beheeromgeving is niet nodig.

Een eventoverzicht, betalingen, ticketing en capaciteitsbeheer vallen buiten de
opdracht. Voor overige details mag je zelf een redelijke keuze maken; licht die
kort toe in je README.

## Oplevering

Lever je code op met een korte README waarin je beschrijft:

- Welke keuzes je hebt gemaakt, met name voor het datamodel en de frontend.
- Wat eventueel nog niet af is en wat je met meer tijd zou verbeteren.

## Beoordeling

We beoordelen op:

- De werking van de eventpagina en de aanmelding.
- De structuur van de backend, het datamodel en de validatie.
- De opzet van de React-componenten en de gegevensoverdracht via Inertia.
- Responsive styling, toegankelijkheid en feedback aan de bezoeker.
- Leesbaarheid, consistentie en gerichte tests.
- Je prioriteiten en de onderbouwing van je keuzes.

Het is niet erg als niet alles volledig is uitgewerkt. Stop na maximaal 8 uur en
geef in bijbehorende documentatie aan waar je staat. Je afwegingen zijn onderdeel van de beoordeling.

## Startpunt

Maak een fork van de voorbeeldrepository met Laravel 13, Inertia en React:

[Daymakers assessment repository](https://github.com/FX-Agency/assesment-daymakers)

Volg de installatie-instructies in `README.md`. De aanwezige accountfunctionaliteit
is geen vereiste voor de eventaanmelding maar mag je eventueel gebruiken.
