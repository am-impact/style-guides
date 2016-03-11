# CSS Style Guide

## Coding Style

- indent met 4 spaties
- Spatie na : bij de properties
- Spatie voor { 
- Multiple selectors elk op een eigen regel
- Elke propertie op een nieuwe regel
- Properties met een 0 value moet *geen* unit hebben (dus 0 en geen 0px)
- Lowercase hex ( bijv #fff )
- Commentblokken met /* */ 
- Commentregels met //
- Gebruik dashes in selectors in plaats van underscores (.my-class, niet .my_class)
- Boven elk scss bestand / component omschrijven waar deze component wordt gebruikt. ( bijv bij .overview: /* Wordt gebruikt bij nieuws- en zoekoverzicht */)
- Mediaqueries zoveel mogelijk gebundeld onderaan een component
- Classes zoveel mogelijk functioneel of contentbenaming geven en niet naar layout ( dus geen class="blue" bijv. )
- Geen id's gebruiken maar classes
- Probeer zo weinig mogelijk element selectors te gebruiken, maar classes. Als een element wijzigt van li naar div bijv, dan geeft dat geen problemen

## Volgorde properties
    .selector {
        /* Positioning */
        position: absolute;
        z-index: 10;
        top: 0;
        right: 0;
        transform: scale(1.5);
        
        /* Display & Box Model */
        display: inline-block;
        overflow: hidden;
        box-sizing: border-box;
        width: 100px;
        height: 100px;
   
        padding: 10px;
        margin: 10px;
        border: 10px solid #333;
        
        /* Text */
        font-family: sans-serif;
        font-size: 16px;
        line-height: 1.4;
        text-align: right;
        
        /* Color */
        background: #000;
        color: #fff;
        
        /* Other */
        cursor: pointer;
        opacity: 1;
        transition: all 0.3s ease;
    }

## BEM
Wij gebruiken de BEM methodologie
[Documentatie](http://getbem.com/naming/)

## Folder structuur
    - scss
    --- bower_components
    --- components
    ------ global
    ------ grid
    ------ nav
    ------ page
    --- generic
    --- libs

- In de `hoofdfolder` staan de te compilen bestanden + _settings.scss
- In `generic` staan globale bestanden zoals functions, mixins, fonts, global enz
- In `components` is er een onderverdeling tussen globale componenten, page componenten, nav componenten en het zurb foundation grid
- Globale componenten zijn componenten die je vaker op een pagina kan gebruiken. Bijv een button


## Variabelen
- Globale variabelen staan in de _settings.scss. Variabelen van een component bovenin een component zetten
- Component variabelen structuur: `$component-style-modifier` (bijv: `$button-background-light`)
