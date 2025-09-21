    #home {
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 15px;
    }

    button {
        background-color: #0077b6;
        color: white;
        padding: 15px 25px;
        font-size: 16px;
        border: none;
        border-radius: 12px;
        cursor: pointer;
        transition: background 0.3s;
        width: 260px;
        text-align: center;
    }

    button:hover {
        background-color: #023e8a;
    }

    .back-btn {
        display: inline-block;
        margin-bottom: 15px;
        padding: 8px 15px;
        background-color: #0077b6;
        color: white;
        border-radius: 8px;
        text-decoration: none;
        font-size: 14px;
        cursor: pointer;
    }

    .back-btn:hover {
        background-color: #023e8a;
    }

    h1 {
        font-size: 24px;
        color: #023e8a;
        margin-bottom: 15px;
    }

    h2 {
        font-size: 18px;
        color: #0077b6;
        margin-top: 20px;
        margin-bottom: 10px;
        border-bottom: 1px solid #0077b6;
        padding-bottom: 3px;
    }

    table {
        width: 100%;
        border-collapse: collapse;
        margin: 10px 0 15px 0;
        font-size: 13px;
    }

    th, td {
        border: 1px solid #0077b6;
        padding: 6px 10px;
        text-align: left;
    }

    th {
        background-color: #0077b6;
        color: white;
    }

    tr:nth-child(even) {
        background-color: #e0f7ff;
    }

    /* Hide all topic sections initially */
    .topic {
        display: none;
    }
</style>
</head>
<body>

<!-- Home Screen -->
<div id="home">
    <button onclick="showCourse('present')">Present tense (regular verbs)</button>
    <button onclick="showCourse('seinHaben')">Sein & haben usage</button>
    <button onclick="showCourse('articles')">Definite/indefinite articles</button>
    <button onclick="showCourse('plurals')">Noun plurals</button>
    <button onclick="showCourse('pronouns')">Personal pronouns</button>
    <button onclick="showCourse('negation')">Basic negation (kein/nicht)</button>
    <button onclick="showCourse('modal')">Modal verbs basics</button>
    <button onclick="showCourse('wordOrder')">Word order in main clause</button>
    <button onclick="showCourse('questions')">Yes/No & W-questions</button>
    <button onclick="showCourse('accusative')">Accusative case basics</button>
</div>

<!-- Present Tense -->
<div id="present" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    
    <h1>Present Tense (Präsens)</h1>

    <p>The present tense (Präsens) in German is used to describe:</p>
    <ul>
        <li>Actions happening now</li>
        <li>Habitual or repeated actions</li>
        <li>General truths or facts</li>
        <li>Future events with a time reference</li>
    </ul>

    <h2>Regular Verb Conjugation</h2>
    <p>Regular verbs (schwache Verben) follow a predictable pattern: remove <strong>-en</strong> from the infinitive and add endings:</p>
    <ul>
        <li>ich – e</li>
        <li>du – st</li>
        <li>er/sie/es – t</li>
        <li>wir – en</li>
        <li>ihr – t</li>
        <li>sie/Sie – en</li>
    </ul>

    <h3>Example: spielen (to play)</h3>
    <table>
        <tr><th>Pronoun</th><th>spielen</th></tr>
        <tr><td>ich</td><td>spiele</td></tr>
        <tr><td>du</td><td>spielst</td></tr>
        <tr><td>er/sie/es</td><td>spielt</td></tr>
        <tr><td>wir</td><td>spielen</td></tr>
        <tr><td>ihr</td><td>spielt</td></tr>
        <tr><td>sie/Sie</td><td>spielen</td></tr>
    </table>

    <h2>50 Common Regular Verbs (Reference)</h2>
    <p>All regular verbs follow the same endings:</p>
    <table>
        <tr>
            <th>Infinitive</th>
            <th>ich</th>
            <th>du</th>
            <th>er/sie/es</th>
            <th>wir</th>
            <th>ihr</th>
            <th>sie/Sie</th>
        </tr>
        <tr><td>arbeiten</td><td>arbeite</td><td>arbeitest</td><td>arbeitet</td><td>arbeiten</td><td>arbeitet</td><td>arbeiten</td></tr>
        <tr><td>baden</td><td>bade</td><td>badest</td><td>badet</td><td>baden</td><td>badet</td><td>baden</td></tr>
        <tr><td>brauchen</td><td>brauche</td><td>brauchst</td><td>braucht</td><td>brauchen</td><td>braucht</td><td>brauchen</td></tr>
        <tr><td>fragen</td><td>frage</td><td>fragst</td><td>fragt</td><td>fragen</td><td>fragt</td><td>fragen</td></tr>
        <tr><td>hören</td><td>höre</td><td>hörst</td><td>hört</td><td>hören</td><td>hört</td><td>hören</td></tr>
        <tr><td>kaufen</td><td>kaufe</td><td>kaufst</td><td>kauft</td><td>kaufen</td><td>kauft</td><td>kaufen</td></tr>
        <tr><td>lernen</td><td>lerne</td><td>lernst</td><td>lernt</td><td>lernen</td><td>lernt</td><td>lernen</td></tr>
        <tr><td>machen</td><td>mache</td><td>machst</td><td>macht</td><td>machen</td><td>macht</td><td>machen</td></tr>
        <tr><td>öffnen</td><td>öffne</td><td>öffnest</td><td>öffnet</td><td>öffnen</td><td>öffnet</td><td>öffnen</td></tr>
        <tr><td>reden</td><td>rede</td><td>redest</td><td>redet</td><td>reden</td><td>redet</td><td>reden</td></tr>
        <tr><td>reisen</td><td>reise</td><td>reist</td><td>reist</td><td>reisen</td><td>reist</td><td>reisen</td></tr>
        <tr><td>sagen</td><td>sage</td><td>sagst</td><td>sagt</td><td>sagen</td><td>sagt</td><td>sagen</td></tr>
        <tr><td>spielen</td><td>spiele</td><td>spielst</td><td>spielt</td><td>spielen</td><td>spielt</td><td>spielen</td></tr>
        <tr><td>stehen</td><td>stehe</td><td>stehst</td><td>steht</td><td>stehen</td><td>steht</td><td>stehen</td></tr>
        <tr><td>tanzen</td><td>tanze</td><td>tanzt</td><td>tanzt</td><td>tanzen</td><td>tanzt</td><td>tanzen</td></tr>
        <tr><td>trinken</td><td>trinke</td><td>trinkst</td><td>trinkt</td><td>trinken</td><td>trinkt</td><td>trinken</td></tr>
        <tr><td>warten</td><td>warte</td><td>wartest</td><td>wartet</td><td>warten</td><td>wartet</td><td>warten</td></tr>
        <tr><td>wohnen</td><td>wohne</td><td>wohnst</td><td>wohnt</td><td>wohnen</td><td>wohnt</td><td>wohnen</td></tr>
        <tr><td>backen</td><td>backe</td><td>bäckst</td><td>backt</td><td>backen</td><td>backt</td><td>backen</td></tr>
        <tr><td>bringen</td><td>bringe</td><td>bringst</td><td>bringt</td><td>bringen</td><td>bringt</td><td>bringen</td></tr>
        <tr><td>danken</td><td>danke</td><td>dankst</td><td>dankt</td><td>danken</td><td>dankt</td><td>danken</td></tr>
        <tr><td>grüßen</td><td>grüße</td><td>grüßt</td><td>grüßt</td><td>grüßen</td><td>grüßt</td><td>grüßen</td></tr>
        <tr><td>heilen</td><td>heile</td><td>heilst</td><td>heilt</td><td>heilen</td><td>heilt</td><td>heilen</td></tr>
        <tr><td>kochen</td><td>koche</td><td>kochst</td><td>kocht</td><td>kochen</td><td>kocht</td><td>kochen</td></tr>
        <tr><td>lachen</td><td>lache</td><td>lachst</td><td>lacht</td><td>lachen</td><td>lacht</td><td>lachen</td></tr>
        <tr><td>lieben</td><td>liebe</td><td>liebst</td><td>liebt</td><td>lieben</td><td>liebt</td><td>lieben</td></tr>
        <tr><td>planen</td><td>plane</td><td>planst</td><td>plant</td><td>planen</td><td>plant</td><td>planen</td></tr>
        <tr><td>stellen</td><td>stelle</td><td>stellst</td><td>stellt</td><td>stellen</td><td>stellt</td><td>stellen</td></tr>
        <tr><td>zeigen</td><td>zeige</td><td>zeigst</td><td>zeigt</td><td>zeigen</td><td>zeigt</td><td>zeigen</td></tr>
        <tr><td>arbeiten</td><td>arbeite</td><td>arbeitest</td><td>arbeitet</td><td>arbeiten</td><td>arbeitet</td><td>arbeiten</td></tr>
        <tr><td>fühlen</td><td>fühle</td><td>fühlst</td><td>fühlt</td><td>fühlen</td><td>fühlt</td><td>fühlen</td></tr>
        <tr><td>gehören</td><td>gehöre</td><td>gehörst</td><td>gehört</td><td>gehören</td><td>gehört</td><td>gehören</td></tr>
        <tr><td>tanzen</td><td>tanze</td><td>tanzt</td><td>tanzt</td><td>tanzen</td><td>tanzt</td><td>tanzen</td></tr>
        <tr><td>wandern</td><td>wandere</td><td>wanderst</td><td>wandert</td><td>wandern</td><td>wandert</td><td>wandern</td></tr>
        <tr><td>zeichnen</td><td>zeichne</td><td>zeichnest</td><td>zeichnet</td><td>zeichnen</td><td>zeichnet</td><td>zeichnen</td></tr>
    </table>

    <h2>Irregular Verbs (Strong Verbs)</h2>
    <p>Irregular verbs have **stem changes** in 2nd and 3rd person singular (du/er/sie/es). Endings remain regular.</p>

    <h3>sehen (to see)</h3>
    <table>
        <tr><th>Pronoun</th><th>sehen</th></tr>
        <tr><td>ich</td><td>sehe</td></tr>
        <tr><td>du</td><td>siehst</td></tr>
        <tr><td>er/sie/es</td><td>sieht</td></tr>
        <tr><td>wir</td><td>sehen</td></tr>
        <tr><td>ihr</td><td>seht</td></tr>
        <tr><td>sie/Sie</td><td>sehen</td></tr>
    </table>

    <h3>fahren (to drive/go)</h3>
    <table>
        <tr><td>ich</td><td>fahre</td></tr>
        <tr><td>du</td><td>fährst</td></tr>
        <tr><td>er/sie/es</td><td>fährt</td></tr>
        <tr><td>wir</td><td>fahren</td></tr>
        <tr><td>ihr</td><td>fahrt</td></tr>
        <tr><td>sie/Sie</td><td>fahren</td></tr>
    </table>

    <h3>sprechen (to speak)</h3>
    <table>
        <tr><td>ich</td><td>spreche</td></tr>
        <tr><td>du</td><td>sprichst</td></tr>
        <tr><td>er/sie/es</td><td>spricht</td></tr>
        <tr><td>wir</td><<td>sprechen</td></tr>
        <tr><td>ihr</td><td>sprecht</td></tr>
        <tr><td>sie/Sie</td><td>sprechen</td></tr>
    </table>

    <h3>lesen (to read)</h3>
    <table>
        <tr><td>ich</td><td>lese</td></tr>
        <tr><td>du</td><td>liest</td></tr>
        <tr><td>er/sie/es</td><td>liest</td></tr>
        <tr><td>wir</td><td>lesen</td></tr>
        <tr><td>ihr</td><td>lest</td></tr>
        <tr><td>sie/Sie</td><td>lesen</td></tr>
    </table>

    <h3>essen (to eat)</h3>
    <table>
        <tr><td>ich</td><td>esse</td></tr>
        <tr><td>du</td><td>isst</td></tr>
        <tr><td>er/sie/es</td><td>isst</td></tr>
        <tr><td>wir</td><td>essen</td></tr>
        <tr><td>ihr</td><td>esst</td></tr>
        <tr><td>sie/Sie</td><td>essen</td></tr>
    </table>

    <h3>laufen (to run)</h3>
    <table>
        <tr><td>ich</td><td>laufe</td></tr>
        <tr><td>du</td><td>läufst</td></tr>
        <tr><td>er/sie/es</td><td>läuft</td></tr>
        <tr><td>wir</td><td>laufen</td></tr>
        <tr><td>ihr</td><td>lauft</td></tr>
        <tr><td>sie/Sie</td><td>laufen</td></tr>
    </table>

    <h2>Usage Examples</h2>
    <ul>
        <li>Ich lerne Deutsch. (I am learning German.)</li>
        <li>Wir gehen jeden Sonntag spazieren. (We go for a walk every Sunday.)</li>
        <li>Ich fahre morgen nach Berlin. (I am traveling to Berlin tomorrow.)</li>
        <li>Er spricht gut Deutsch. (He speaks German well.)</li>
        <li>Die Sonne scheint. (The sun is shining.)</li>
        <li>Du liest ein interessantes Buch. (You are reading an interesting book.)</li>
        <li>Wir spielen Fußball im Park. (We play football in the park.)</li>
        <li>Sie läuft schnell zum Bus. (She runs fast to the bus.)</li>
        <li>Wir essen zusammen Abendessen. (We eat dinner together.)</li>
        <li>Er sieht den Film im Kino. (He sees the movie in the cinema.)</li>
    </ul>
    <h2>Irregular Verbs – Stem Change Patterns in Präsens</h2>

<!-- 1st Pattern: e → i -->
<h3>1. e → i (du/er/sie/es)</h3>
<p>In some verbs, the stem vowel <strong>e</strong> changes to <strong>i</strong> in <strong>du</strong> and <strong>er/sie/es</strong>.</p>

<h4>Example: sprechen (to speak)</h4>
<table>
    <tr><th>Pronoun</th><th>Conjugation</th></tr>
    <tr><td>ich</td><td>spreche</td></tr>
    <tr><td>du</td><td>sprichst</td></tr>
    <tr><td>er/sie/es</td><td>spricht</td></tr>
    <tr><td>wir</td><td>sprechen</td></tr>
    <tr><td>ihr</td><td>sprecht</td></tr>
    <tr><td>sie/Sie</td><td>sprechen</td></tr>
</table>

<p>Other common verbs with <strong>e → i</strong>:</p>
<ul>
    <li>geben (to give)</li>
    <li>nehmen (to take)</li>
    <li>essen (to eat)</li>
    <li>treffen (to meet)</li>
    <li>vergessen (to forget)</li>
</ul>

<!-- 2nd Pattern: e → ie -->
<h3>2. e → ie (du/er/sie/es)</h3>
<p>Some verbs change <strong>e</strong> to <strong>ie</strong> in <strong>du</strong> and <strong>er/sie/es</strong>.</p>

<h4>Example: lesen (to read)</h4>
<table>
    <tr><th>Pronoun</th><th>Conjugation</th></tr>
    <tr><td>ich</td><td>lese</td></tr>
    <tr><td>du</td><td>liest</td></tr>
    <tr><td>er/sie/es</td><td>liest</td></tr>
    <tr><td>wir</td><td>lesen</td></tr>
    <tr><td>ihr</td><td>lest</td></tr>
    <tr><td>sie/Sie</td><td>lesen</td></tr>
</table>

<p>Other common verbs with <strong>e → ie</strong>:</p>
<ul>
    <li>sehen (to see)</li>
    <li>verstehen (to understand)</li>
    <li>empfehlen (to recommend)</li>
    <li>gefallen (to please)</li>
    <li>lesen (to read)</li>
</ul>

<!-- 3rd Pattern: a → ä -->
<h3>3. a → ä (du/er/sie/es)</h3>
<p>Some verbs change <strong>a</strong> to <strong>ä</strong> in <strong>du</strong> and <strong>er/sie/es</strong>.</p>

<h4>Example: fahren (to go/drive)</h4>
<table>
    <tr><th>Pronoun</th><th>Conjugation</th></tr>
    <tr><td>ich</td><td>fahre</td></tr>
    <tr><td>du</td><td>fährst</td></tr>
    <tr><td>er/sie/es</td><td>fährt</td></tr>
    <tr><td>wir</td><td>fahren</td></tr>
    <tr><td>ihr</td><td>fahrt</td></tr>
    <tr><td>sie/Sie</td><td>fahren</td></tr>
</table>

<p>Other common verbs with <strong>a → ä</strong>:</p>
<ul>
    <li>laufen (to run)</li>
    <li>schlafen (to sleep)</li>
    <li>tragen (to carry/wear)</li>
    <li>halten (to hold)</li>
    <li>waschen (to wash)</li>
</ul>

<!-- 4th Pattern: au → äu -->
<h3>4. au → äu (du/er/sie/es)</h3>
<p>Some verbs change <strong>au</strong> to <strong>äu</strong> in <strong>du</strong> and <strong>er/sie/es</strong>.</p>

<h4>Example: laufen (to run)</h4>
<table>
    <tr><th>Pronoun</th><th>Conjugation</th></tr>
    <tr><td>ich</td><td>laufe</td></tr>
    <tr><td>du</td><td>läufst</td></tr>
    <tr><td>er/sie/es</td><td>läuft</td></tr>
    <tr><td>wir</td><td>laufen</td></tr>
    <tr><td>ihr</td><td>lauft</td></tr>
    <tr><td>sie/Sie</td><td>laufen</td></tr>
</table>

<p>Other common verbs with <strong>au → äu</strong>:</p>
<ul>
    <li>laufen (to run)</li>
    <li>laufen (repetition of same type)</li>
</ul>
    
    
</div>
        
        
        
        
        
        
 
</div>

<!-- Sein & Haben -->
<div id="seinHaben" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Sein & Haben</h1>
    

<h2>Definition</h2>
<p>
"Sein" means <strong>to be</strong> in English. It is used to describe identity, states, locations, and characteristics.  
"Haben" means <strong>to have</strong> in English. It is used to express possession, age, and certain idiomatic expressions.
</p>

<h2>Conjugation</h2>

<h3>Sein – Present Tense</h3>
<table border="1" cellpadding="5" cellspacing="0">
<tr><th>Pronoun</th><th>Conjugation</th></tr>
<tr><td>ich</td><td>bin</td></tr>
<tr><td>du</td><td>bist</td></tr>
<tr><td>er/sie/es</td><td>ist</td></tr>
<tr><td>wir</td><td>sind</td></tr>
<tr><td>ihr</td><td>seid</td></tr>
<tr><td>sie/Sie</td><td>sind</td></tr>
</table>

<h3>Haben – Present Tense</h3>
<table border="1" cellpadding="5" cellspacing="0">
<tr><th>Pronoun</th><th>Conjugation</th></tr>
<tr><td>ich</td><td>habe</td></tr>
<tr><td>du</td><td>hast</td></tr>
<tr><td>er/sie/es</td><td>hat</td></tr>
<tr><td>wir</td><td>haben</td></tr>
<tr><td>ihr</td><td>habt</td></tr>
<tr><td>sie/Sie</td><td>haben</td></tr>
</table>

<h2>Usage</h2>
<p><strong>Sein</strong> is used for:</p>
<ul>
<li>Identity: Ich bin Lehrer. (I am a teacher.)</li>
<li>Location: Er ist zu Hause. (He is at home.)</li>
<li>State / Condition: Wir sind müde. (We are tired.)</li>
</ul>

<p><strong>Haben</strong> is used for:</p>
<ul>
<li>Possession: Ich habe ein Auto. (I have a car.)</li>
<li>Age: Sie hat 20 Jahre. (She is 20 years old.)</li>
<li>Expressions: Wir haben Zeit. (We have time.)</li>
</ul>

<h2>Examples</h2>
<p><strong>Sein:</strong></p>
<ul>
<li>Ich bin müde. (I am tired.)</li>
<li>Er ist mein Freund. (He is my friend.)</li>
<li>Wir sind im Park. (We are in the park.)</li>
</ul>

<p><strong>Haben:</strong></p>
<ul>
<li>Ich habe einen Hund. (I have a dog.)</li>
<li>Du hast ein Buch. (You have a book.)</li>
<li>Sie hat viele Fragen. (She has many questions.)</li>
</ul>

<h2>Common Verbs / Expressions with Haben</h2>
<table border="1" cellpadding="5" cellspacing="0">
<tr><th>Haben + Verb/Expression</th><th>English Meaning</th></tr>
<tr><td>haben Hunger</td><td>to be hungry</td></tr>
<tr><td>haben Durst</td><td>to be thirsty</td></tr>
<tr><td>haben Angst</td><td>to be afraid</td></tr>
<tr><td>haben Zeit</td><td>to have time</td></tr>
<tr><td>haben Lust</td><td>to feel like</td></tr>
<tr><td>haben Recht</td><td>to be right</td></tr>
<tr><td>haben Spaß</td><td>to have fun</td></tr>
<tr><td>haben Interesse</td><td>to be interested</td></tr>
<tr><td>haben Sorgen</td><td>to worry</td></tr>
<tr><td>haben Erfolg</td><td>to have success</td></tr>
<tr><td>haben Geduld</td><td>to have patience</td></tr>
<tr><td>haben Angst vor</td><td>to be afraid of</td></tr>
<tr><td>haben Geburtstag</td><td>to have a birthday</td></tr>
<tr><td>haben Besuch</td><td>to have visitors</td></tr>
<tr><td>haben Platz</td><td>to have space</td></tr>
<tr><td>haben Sorgen um</td><td>to worry about</td></tr>
<tr><td>haben Recht auf</td><td>to have the right to</td></tr>
<tr><td>haben Lust auf</td><td>to feel like</td></tr>
<tr><td>haben Geduld mit</td><td>to have patience with</td></tr>
<tr><td>haben Vertrauen</td><td>to have trust</td></tr>
<tr><td>haben Hoffnung</td><td>to have hope</td></tr>
<tr><td>haben Spaß an</td><td>to enjoy</td></tr>
<tr><td>haben Freude</td><td>to have joy</td></tr>
<tr><td>haben Respekt</td><td>to have respect</td></tr>
<tr><td>haben Einfluss</td><td>to have influence</td></tr>
<tr><td>haben Rechtfertigung</td><td>to have justification</td></tr>
<tr><td>haben Vorstellung</td><td>to have idea / concept</td></tr>
<tr><td>haben Erfolg bei</td><td>to succeed at</td></tr>
<tr><td>haben Kontakt</td><td>to have contact</td></tr>
<tr><td>haben Zugang</td><td>to have access</td></tr>
<tr><td>haben Gelegenheit</td><td>to have opportunity</td></tr>
<tr><td>haben Probleme</td><td>to have problems</td></tr>
<tr><td>haben Verantwortung</td><td>to have responsibility</td></tr>
<tr><td>haben Kontrolle</td><td>to have control</td></tr>
<tr><td>haben Einfluss auf</td><td>to influence</td></tr>
<tr><td>haben Fehler</td><td>to make mistakes</td></tr>
<tr><td>haben Erfahrung</td><td>to have experience</td></tr>
<tr><td>haben Verpflichtung</td><td>to have obligation</td></tr>
<tr><td>haben Bedeutung</td><td>to have meaning</td></tr>
<tr><td>haben Chance</td><td>to have chance</td></tr>
<tr><td>haben Eindruck</td><td>to have impression</td></tr>
<tr><td>haben Kontakt zu</td><td>to have contact with</td></tr>
<tr><td>haben Kontrolle über</td><td>to have control over</td></tr>
<tr><td>haben Recht auf</td><td>to have right to</td></tr>
<tr><td>haben Erfolg mit</td><td>to succeed with</td></tr>
<tr><td>haben Spaß mit</td><td>to have fun with</td></tr>
<tr><td>haben Freundschaft</td><td>to have friendship</td></tr>
<tr><td>haben Interesse an</td><td>to be interested in</td></tr>
<tr><td>haben Wissen</td><td>to have knowledge</td></tr>
<tr><td>haben Macht</td><td>to have power</td></tr>
<tr><td>haben Kontrolle</td><td>to have control</td></tr>
<tr><td>haben Kontakt zu</td><td>to have contact with</td></tr>
<tr><td>haben Anteil</td><td>to have share / part</td></tr>
</table>

<h2>Common Verbs / Expressions with Sein</h2>
<table border="1" cellpadding="5" cellspacing="0">
<tr><th>Sein + Expression</th><th>English Meaning</th></tr>
<tr><td>sein müde</td><td>to be tired</td></tr>
<tr><td>sein glücklich</td><td>to be happy</td></tr>
<tr><td>sein krank</td><td>to be sick</td></tr>
<tr><td>sein bereit</td><td>to be ready</td></tr>
<tr><td>sein beschäftigt</td><td>to be busy</td></tr>
<tr><td>sein traurig</td><td>to be sad</td></tr>
<tr><td>sein nervös</td><td>to be nervous</td></tr>
<tr><td>sein hungrig</td><td>to be hungry</td></tr>
<tr><td>sein durstig</td><td>to be thirsty</td></tr>
<tr><td>sein zu Hause</td><td>to be at home</td></tr>
<tr><td>sein unterwegs</td><td>to be on the way</td></tr>
<tr><td>sein im Büro</td><td>to be in the office</td></tr>
<tr><td>sein im Park</td><td>to be in the park</td></tr>
<tr><td>sein im Kino</td><td>to be in the cinema</td></tr>
<tr><td>sein frei</td><td>to be free</td></tr>
<tr><td>sein beschäftigt mit</td><td>to be busy with</td></tr>
<tr><td>sein traurig über</td><td>to be sad about</td></tr>
<tr><td>sein stolz auf</td><td>to be proud of</td></tr>
<tr><td>sein sicher</td><td>to be sure</td></tr>
<tr><td>sein verantwortlich</td><td>to be responsible</td></tr>
<tr><td>sein interessiert an</td><td>to be interested in</td></tr>
<tr><td>sein bekannt</td><td>to be known</td></tr>
<tr><td>sein beliebt</td><td>to be popular</td></tr>
<tr><td>sein bereit für</td><td>to be ready for</td></tr>
<tr><td>sein enttäuscht</td><td>to be disappointed</td></tr>
<tr><td>sein verrückt</td><td>to be crazy</td></tr>
<tr><td>sein ruhig</td><td>to be calm</td></tr>
<tr><td>sein nervös wegen</td><td>to be nervous about</td></tr>
<tr><td>sein stolz auf</td><td>to be proud of</td></tr>
<tr><td>sein müde von</td><td>to be tired from</td></tr>
<tr><td>sein zufrieden</td><td>to be satisfied</td></tr>
<tr><td>sein verliebt</td><td>to be in love</td></tr>
<tr><td>sein sicher über</td><td>to be sure about</td></tr>
<tr><td>sein vorbereitet</td><td>to be prepared</td></tr>
<tr><td>sein beschäftigt mit</td><td>to be busy with</td></tr>
<tr><td>sein verantwortlich für</td><td>to be responsible for</td></tr>
<tr><td>sein begeistert von</td><td>to be excited about</td></tr>
<tr><td>sein traurig wegen</td><td>to be sad because of</td></tr>
<tr><td>sein erstaunt</td><td>to be amazed</td></tr>
<tr><td>sein interessiert an</td><td>to be interested in</td></tr>
<tr><td>sein enttäuscht von</td><td>to be disappointed by</td></tr>
<tr><td>sein glücklich über</td><td>to be happy about</td></tr>
<tr><td>sein bekannt für</td><td>to be known for</td></tr>
<tr><td>sein beliebt bei</td><td>to be popular with</td></tr>
<tr><td>sein verantwortlich für</td><td>to be responsible for</td></tr>
<tr><td>sein stolz auf</td><td>to be proud of</td></tr>
<tr><td>sein zufrieden mit</td><td>to be satisfied with</td></tr>
<tr><td>sein erstaunt über</td><td>to be amazed about</td></tr>
<tr><td>sein wütend auf</td><td>to be angry at</td></tr>
<tr><td>sein verliebt in</td><td>to be in love with</td></tr>
<tr><td>sein überzeugt von</td><td>to be convinced of</td></tr>
</table>
<div id="seinHaben">

<h1>here is list of sein and haben verb</h1>

<h2>50 Sein Verbs (motion/change-of-state) </h2>
<table border="1" cellpadding="4" cellspacing="0">
<tr><th>Verb</th><th>Meaning</th><th>Verb</th><th>Meaning</th></tr>
<tr><td>fahren</td><td>to drive/go</td><td>gehen</td><td>to go/walk</td></tr>
<tr><td>kommen</td><td>to come</td><td>bleiben</td><td>to stay</td></tr>
<tr><td>laufen</td><td>to run</td><td>fliegen</td><td>to fly</td></tr>
<tr><td>reisen</td><td>to travel</td><td>schwimmen</td><td>to swim</td></tr>
<tr><td>fallen</td><td>to fall</td><td>steigen</td><td>to climb/rise</td></tr>
<tr><td>aufstehen</td><td>to get up</td><td>einschlafen</td><td>to fall asleep</td></tr>
<tr><td>ankommen</td><td>to arrive</td><td>zurückkommen</td><td>to come back</td></tr>
<tr><td>abfahren</td><td>to depart</td><td>umziehen</td><td>to move house</td></tr>
<tr><td>aufwachen</td><td>to wake up</td><td>beginnen</td><td>to begin</td></tr>
<tr><td>wachsen</td><td>to grow</td><td>sterben</td><td>to die</td></tr>
<tr><td>passieren</td><td>to happen</td><td>eintreten</td><td>to enter</td></tr>
<tr><td>zurückkehren</td><td>to return</td><td>ziehen</td><td>to pull/move</td></tr>
<tr><td>verschwinden</td><td>to disappear</td><td>klettern</td><td>to climb</td></tr>
<tr><td>fallen lassen</td><td>to drop</td><td>umkehren</td><td>to turn back</td></tr>
<tr><td>reiten</td><td>to ride (horse)</td><td>absteigen</td><td>to get off/dismount</td></tr>
<tr><td>ansteigen</td><td>to rise/increase</td><td>hineingehen</td><td>to go in</td></tr>
<tr><td>hinausgehen</td><td>to go out</td><td>mitkommen</td><td>to come along</td></tr>
<tr><td>losgehen</td><td>to set off/start</td><td>zurückgehen</td><td>to go back</td></tr>
<tr><td>fortgehen</td><td>to leave/go away</td><td>umfallen</td><td>to fall over</td></tr>
<tr><td>herunterkommen</td><td>to come down</td><td>vorankommen</td><td>to make progress</td></tr>
</table>

<h2>50 Haben Verbs (transitive/actions) – Two per row</h2>
<table border="1" cellpadding="4" cellspacing="0">
<tr><th>Verb</th><th>Meaning</th><th>Verb</th><th>Meaning</th></tr>
<tr><td>haben</td><td>to have</td><td>spielen</td><td>to play</td></tr>
<tr><td>machen</td><td>to do/make</td><td>lernen</td><td>to learn</td></tr>
<tr><td>arbeiten</td><td>to work</td><td>kaufen</td><td>to buy</td></tr>
<tr><td>verkaufen</td><td>to sell</td><td>lesen</td><td>to read</td></tr>
<tr><td>schreiben</td><td>to write</td><td>kochen</td><td>to cook</td></tr>
<tr><td>trinken</td><td>to drink</td><td>essen</td><td>to eat</td></tr>
<tr><td>singen</td><td>to sing</td><td>tanzen</td><td>to dance</td></tr>
<tr><td>besuchen</td><td>to visit</td><td>verstehen</td><td>to understand</td></tr>
<tr><td>erklären</td><td>to explain</td><td>fragen</td><td>to ask</td></tr>
<tr><td>antworten</td><td>to answer</td><td>brauchen</td><td>to need</td></tr>
<tr><td>vergessen</td><td>to forget</td><td>erinnern</td><td>to remember</td></tr>
<tr><td>verlieren</td><td>to lose</td><td>gewinnen</td><td>to win</td></tr>
<tr><td>zeigen</td><td>to show</td><td>öffnen</td><td>to open</td></tr>
<tr><td>schließen</td><td>to close</td><td>finden</td><td>to find</td></tr>
<tr><td>bezahlen</td><td>to pay</td><td>vorbereiten</td><td>to prepare</td></tr>
<tr><td>bestellen</td><td>to order/request</td><td>sagen</td><td>to say/tell</td></tr>
<tr><td>genießen</td><td>to enjoy</td><td>verbessern</td><td>to improve</td></tr>
<tr><td>besuchen</td><td>to attend</td><td>messen</td><td>to measure</td></tr>
<tr><td>betrachten</td><td>to consider/look at</td><td>anbieten</td><td>to offer</td></tr>
<tr><td>fotografieren</td><td>to photograph</td><td>planen</td><td>to plan</td></tr>
<tr><td>vermissen</td><td>to miss</td><td>erfahren</td><td>to experience</td></tr>
<tr><td>benutzen</td><td>to use</td><td>kosten</td><td>to cost</td></tr>
<tr><td>vorbereiten</td><td>to get ready/prepare</td><td>zeigen</td><td>to show</td></tr>
<tr><td>erklären</td><td>to clarify</td><td>genießen</td><td>to enjoy</td></tr>
<tr><td>arbeiten</td><td>to work</td><td>lesen</td><td>to read</td></tr>
<tr><td>schreiben</td><td>to write</td><td>kaufen</td><td>to buy</td></tr>
<tr><td>bezahlen</td><td>to pay</td><td>bestellen</td><td>to order</td></tr>
<tr><td>besuchen</td><td>to visit</td><td>lernen</td><td>to learn</td></tr>
</table>

</div>

</div>
</div>

<!-- Articles -->
<div id="articles" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Definite/Indefinite Articles</h1>
    

    <h2>1. Introduction</h2>
    <p>
        Articles are words placed before nouns to indicate specificity, gender, number, and case.
        German has <strong>definite articles</strong> (der, die, das) and <strong>indefinite articles</strong> (ein, eine, ein).
        Correct usage is crucial because articles change with gender, number, and grammatical case.
    </p>

    <h2>2. Definite Articles (Der, Die, Das)</h2>
    <p>
        <strong>Definition:</strong> Used for specific nouns.<br>
        <strong>Genders & Typical Endings:</strong><br>
        <ul>
            <li><strong>Masculine (der):</strong> nouns often end in -er, -en, -el, -ig, -ling</li>
            <li><strong>Feminine (die):</strong> nouns often end in -e, -heit, -keit, -ung, -schaft, -ion, -tät</li>
            <li><strong>Neuter (das):</strong> nouns often end in -chen, -lein, -ment, -um, -tum, -ma</li>
            <li><strong>Plural:</strong> die (all genders)</li>
        </ul>
    </p>

    <h3>Examples</h3>
    <ul>
        <li>der Mann – the man</li>
        <li>die Frau – the woman</li>
        <li>das Kind – the child</li>
        <li>die Kinder – the children</li>
    </ul>

    <h2>3. Indefinite Articles (Ein, Eine)</h2>
    <p>
        <strong>Definition:</strong> Used for non-specific nouns.<br>
        <strong>Genders:</strong><br>
        <ul>
            <li>Masculine: ein</li>
            <li>Feminine: eine</li>
            <li>Neuter: ein</li>
            <li>Plural: – (use keine for negation)</li>
        </ul>
    </p>

    <h3>Examples</h3>
    <ul>
        <li>ein Mann – a man</li>
        <li>eine Frau – a woman</li>
        <li>ein Kind – a child</li>
    </ul>

    <h2>4. Articles Across All Cases with Endings</h2>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>Case</th>
            <th>Gender</th>
            <th>Definite Article</th>
            <th>Indefinite Article</th>
            <th>Noun Ending / Notes</th>
        </tr>
        <tr><td rowspan="4">Nominative</td><td>Masculine</td><td>der</td><td>ein</td><td>-er, -en, -el, -ig, -ling</td></tr>
        <tr><td>Feminine</td><td>die</td><td>eine</td><td>-e, -heit, -keit, -ung, -schaft, -ion, -tät</td></tr>
        <tr><td>Neuter</td><td>das</td><td>ein</td><td>-chen, -lein, -ment, -um, -tum, -ma</td></tr>
        <tr><td>Plural</td><td>die</td><td>–</td><td>all genders plural</td></tr>

        <tr><td rowspan="4">Accusative</td><td>Masculine</td><td>den</td><td>einen</td><td>Add -en if noun changes</td></tr>
        <tr><td>Feminine</td><td>die</td><td>eine</td><td>Same as nominative</td></tr>
        <tr><td>Neuter</td><td>das</td><td>ein</td><td>Same as nominative</td></tr>
        <tr><td>Plural</td><td>die</td><td>–</td><td>Add -n if noun allows</td></tr>

        <tr><td rowspan="4">Dative</td><td>Masculine</td><td>dem</td><td>einem</td><td>Add -m to article, noun may stay same</td></tr>
        <tr><td>Feminine</td><td>der</td><td>einer</td><td>Add -r to article</td></tr>
        <tr><td>Neuter</td><td>dem</td><td>einem</td><td>Add -m to article</td></tr>
        <tr><td>Plural</td><td>den</td><td>–</td><td>Add -n to noun if not ending in -n</td></tr>

        <tr><td rowspan="4">Genitive</td><td>Masculine</td><td>des</td><td>eines</td><td>Add -s/-es to noun</td></tr>
        <tr><td>Feminine</td><td>der</td><td>einer</td><td>No noun ending change</td></tr>
        <tr><td>Neuter</td><td>des</td><td>eines</td><td>Add -s/-es to noun</td></tr>
        <tr><td>Plural</td><td>der</td><td>–</td><td>No noun ending change</td></tr>
    </table>

    <h2>5. Rules & Tips</h2>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Rule / Tip</th><th>Explanation</th></tr>
        <tr><td>Masculine nouns</td><td>Often end in -er, -en, -el, -ig, -ling → der</td></tr>
        <tr><td>Feminine nouns</td><td>Often end in -e, -heit, -keit, -ung, -schaft, -ion, -tät → die</td></tr>
        <tr><td>Neuter nouns</td><td>Often end in -chen, -lein, -ment, -um, -tum, -ma → das</td></tr>
        <tr><td>Plurals</td><td>Always take die, regardless of gender</td></tr>
        <tr><td>Indefinite articles</td><td>Do not exist in plural; use keine for negation</td></tr>
        <tr><td>Dative Plural</td><td>Add -n to noun if it doesn’t already end in -n</td></tr>
        <tr><td>Genitive Masculine/Neuter</td><td>Add -s or -es to noun depending on ending</td></tr>
        <tr><td>Memorization Tip</td><td>Learn article + noun together (der Tisch, die Lampe, das Buch)</td></tr>
        <tr><td>Special Cases</td><td>Some nouns have irregular gender; always check a dictionary</td></tr>
        <tr><td>Consistency</td><td>Check article whenever using noun in different cases</td></tr>
    </table>

    <h2>6. Summary</h2>
    <p>
        Definite articles = der, die, das → specific nouns<br>
        Indefinite articles = ein, eine → non-specific nouns<br>
        Always consider gender, number, and case for correct usage<br>
        Learn common noun endings to guess articles correctly<br>
        Practice regularly with nouns in different cases
        
<div id="der-nouns">
    <h1>Masculine Nouns (Der) – 50+ Examples from Various Fields</h1>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>German</th>
            <th>English</th>
            <th>German</th>
            <th>English</th>
        </tr>
        <tr><td>der Sommer</td><td>the summer</td><td>der Winter</td><td>the winter</td></tr>
        <tr><td>der Frühling</td><td>the spring</td><td>der Herbst</td><td>the autumn</td></tr>
        <tr><td>der Regen</td><td>the rain</td><td>der Schnee</td><td>the snow</td></tr>
        <tr><td>der Wind</td><td>the wind</td><td>der Sturm</td><td>the storm</td></tr>
        <tr><td>der Präsident</td><td>the president</td><td>der Politiker</td><td>the politician</td></tr>
        <tr><td>der Minister</td><td>the minister</td><td>der Bürgermeister</td><td>the mayor</td></tr>
        <tr><td>der Lehrer</td><td>the teacher</td><td>der Schüler</td><td>the student</td></tr>
        <tr><td>der Professor</td><td>the professor</td><td>der Direktor</td><td>the principal/director</td></tr>
        <tr><td>der Bahnhof</td><td>the train station</td><td>der Flughafen</td><td>the airport</td></tr>
        <tr><td>der Park</td><td>the park</td><td>der Garten</td><td>the garden</td></tr>
        <tr><td>der Wald</td><td>the forest</td><td>der Berg</td><td>the mountain</td></tr>
        <tr><td>der Fluss</td><td>the river</td><td>der Ozean</td><td>the ocean</td></tr>
        <tr><td>der See</td><td>the lake</td><td>der Hügel</td><td>the hill</td></tr>
        <tr><td>der Himmel</td><td>the sky</td><td>der Mond</td><td>the moon</td></tr>
        <tr><td>der Stern</td><td>the star</td><td>der Planet</td><td>the planet</td></tr>
        <tr><td>der Schlüssel</td><td>the key</td><td>der Tisch</td><td>the table</td></tr>
        <tr><td>der Stuhl</td><td>the chair</td><td>der Computer</td><td>the computer</td></tr>
        <tr><td>der Laptop</td><td>the laptop</td><td>der Brief</td><td>the letter</td></tr>
        <tr><td>der Ball</td><td>the ball</td><td>der Film</td><td>the movie</td></tr>
        <tr><td>der Zug</td><td>the train</td><td>der Bus</td><td>the bus</td></tr>
        <tr><td>der Tourist</td><td>the tourist</td><td>der Reiseführer</td><td>the tour guide/book</td></tr>
        <tr><td>der Arzt</td><td>the doctor</td><td>der Musiker</td><td>the musician</td></tr>
        <tr><td>der Künstler</td><td>the artist</td><td>der Schauspieler</td><td>the actor</td></tr>
        <tr><td>der Sänger</td><td>the singer</td><td>der Tänzer</td><td>the dancer</td></tr>
        <tr><td>der Koch</td><td>the cook</td><td>der Bäcker</td><td>the baker</td></tr>
        <tr><td>der Metzger</td><td>the butcher</td><td>der Verkäufer</td><td>the shopkeeper</td></tr>
        <tr><td>der Polizist</td><td>the policeman</td><td>der Soldat</td><td>the soldier</td></tr>
        <tr><td>der Wissenschaftler</td><td>the scientist</td><td>der Forscher</td><td>the researcher</td></tr>
        <tr><td>der Pilot</td><td>the pilot</td><td>der Kapitän</td><td>the captain</td></tr>
        <tr><td>der Programmierer</td><td>the programmer</td><td>der Techniker</td><td>the technician</td></tr>
        <tr><td>der Architekt</td><td>the architect</td><td>der Ingenieur</td><td>the engineer</td></tr>
        <tr><td>der Bauer</td><td>the farmer</td><td>der Gärtner</td><td>the gardener</td></tr>
        <tr><td>der Friseur</td><td>the hairdresser</td><td>der Fotograf</td><td>the photographer</td></tr>
        <tr><td>der Lehrer</td><td>the teacher</td><td>der Student</td><td>the student</td></tr>
    </table>
<div id="die-nouns">
    <h1>Feminine Nouns (Die) – 50+ Examples from Various Fields</h1>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>German</th>
            <th>English</th>
            <th>German</th>
            <th>English</th>
        </tr>
        <tr><td>die Sonne</td><td>the sun</td><td>die Wolke</td><td>the cloud</td></tr>
        <tr><td>die Nacht</td><td>the night</td><td>die Woche</td><td>the week</td></tr>
        <tr><td>die Stunde</td><td>the hour</td><td>die Minute</td><td>the minute</td></tr>
        <tr><td>die Schule</td><td>the school</td><td>die Universität</td><td>the university</td></tr>
        <tr><td>die Bibliothek</td><td>the library</td><td>die Klasse</td><td>the class</td></tr>
        <tr><td>die Lehrerin</td><td>the female teacher</td><td>die Schülerin</td><td>the female student</td></tr>
        <tr><td>die Regierung</td><td>the government</td><td>die Partei</td><td>the political party</td></tr>
        <tr><td>die Stadt</td><td>the city</td><td>die Brücke</td><td>the bridge</td></tr>
        <tr><td>die Straße</td><td>the street</td><td>die Kirche</td><td>the church</td></tr>
        <tr><td>die Burg</td><td>the castle</td><td>die Sehenswürdigkeit</td><td>the tourist attraction</td></tr>
        <tr><td>die Blume</td><td>the flower</td><td>die Pflanze</td><td>the plant</td></tr>
        <tr><td>die Wiese</td><td>the meadow</td><td>die Insel</td><td>the island</td></tr>
        <tr><td>die Küste</td><td>the coast</td><td>die Natur</td><td>the nature</td></tr>
        <tr><td>die Lampe</td><td>the lamp</td><td>die Uhr</td><td>the clock</td></tr>
        <tr><td>die Tasche</td><td>the bag</td><td>die Zeitung</td><td>the newspaper</td></tr>
        <tr><td>die Tür</td><td>the door</td><td>die Wand</td><td>the wall</td></tr>
        <tr><td>die Bank</td><td>the bench / bank</td><td>die Brille</td><td>the glasses</td></tr>
        <tr><td>die Jacke</td><td>the jacket</td><td>die Hose</td><td>the pants</td></tr>
        <tr><td>die Frau</td><td>the woman</td><td>die Tochter</td><td>the daughter</td></tr>
        <tr><td>die Mutter</td><td>the mother</td><td>die Schwester</td><td>the sister</td></tr>
        <tr><td>die Tante</td><td>the aunt</td><td>die Nichte</td><td>the niece</td></tr>
        <tr><td>die Freundin</td><td>the female friend</td><td>die Kollegin</td><td>the female colleague</td></tr>
        <tr><td>die Ärztin</td><td>the female doctor</td><td>die Sängerin</td><td>the female singer</td></tr>
        <tr><td>die Schauspielerin</td><td>the actress</td><td>die Musikerin</td><td>the female musician</td></tr>
        <tr><td>die Köchin</td><td>the female cook</td><td>die Bäckerin</td><td>the female baker</td></tr>
        <tr><td>die Verkäuferin</td><td>the female shopkeeper</td><td>die Polizistin</td><td>the female policeman</td></tr>
        <tr><td>die Lehrerin</td><td>the teacher (female)</td><td>die Studentin</td><td>the student (female)</td></tr>
        <tr><td>die Wissenschaftlerin</td><td>the female scientist</td><td>die Forscherin</td><td>the female researcher</td></tr>
        <tr><td>die Pilotin</td><td>the female pilot</td><td>die Kapitänin</td><td>the female captain</td></tr>
    </table>
<div id="das-nouns">
    <h1>Neuter Nouns (Das) – 50+ Examples</h1>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>German</th>
            <th>English</th>
            <th>German</th>
            <th>English</th>
        </tr>
        <tr><td>das Auto</td><td>the car</td><td>das Auge</td><td>the eye</td></tr>
        <tr><td>das Baby</td><td>the baby</td><td>das Buch</td><td>the book</td></tr>
        <tr><td>das Bett</td><td>the bed</td><td>das Bild</td><td>the picture</td></tr>
        <tr><td>das Fahrrad</td><td>the bicycle</td><td>das Fenster</td><td>the window</td></tr>
        <tr><td>das Feuer</td><td>the fire</td><td>das Flugzeug</td><td>the airplane</td></tr>
        <tr><td>das Formular</td><td>the form/document</td><td>das Fest</td><td>the festival</td></tr>
        <tr><td>das Feld</td><td>the field</td><td>das Fahrzeug</td><td>the vehicle</td></tr>
        <tr><td>das Foto</td><td>the photo</td><td>das Fernsehen</td><td>the television</td></tr>
        <tr><td>das Fräulein</td><td>the young lady</td><td>das Fisch</td><td>the fish</td></tr>
        <tr><td>das Gesicht</td><td>the face</td><td>das Geschäft</td><td>the shop/business</td></tr>
        <tr><td>das Geld</td><td>the money</td><td>das Gemälde</td><td>the painting</td></tr>
        <tr><td>das Gebäude</td><td>the building</td><td>das Geschenk</td><td>the gift</td></tr>
        <tr><td>das Gras</td><td>the grass</td><td>das Hotel</td><td>the hotel</td></tr>
        <tr><td>das Haus</td><td>the house</td><td>das Heft</td><td>the notebook</td></tr>
        <tr><td>das Hemd</td><td>the shirt</td><td>das Handy</td><td>the mobile phone</td></tr>
        <tr><td>das Hobby</td><td>the hobby</td><td>das Instrument</td><td>the instrument</td></tr>
        <tr><td>das Jahr</td><td>the year</td><td>das Jugendzentrum</td><td>the youth center</td></tr>
        <tr><td>das Krankenhaus</td><td>the hospital</td><td>das Kino</td><td>the cinema</td></tr>
        <tr><td>das Kleid</td><td>the dress</td><td>das Kind</td><td>the child</td></tr>
        <tr><td>das Konzert</td><td>the concert</td><td>das Kunstwerk</td><td>the artwork</td></tr>
        <tr><td>das Kaufhaus</td><td>the department store</td><td>das Lebensmittel</td><td>the grocery/food</td></tr>
        <tr><td>das Leuchtturm</td><td>the lighthouse</td><td>das Messer</td><td>the knife</td></tr>
        <tr><td>das Museum</td><td>the museum</td><td>das Meer</td><td>the sea</td></tr>
        <tr><td>das Meerestier</td><td>the sea animal</td><td>das Mikrofon</td><td>the microphone</td></tr>
        <tr><td>das Mittagessen</td><td>the lunch</td><td>das Mineralwasser</td><td>the mineral water</td></tr>
        <tr><td>das Obst</td><td>the fruit</td><td>das Öl</td><td>the oil</td></tr>
        <tr><td>das Papier</td><td>the paper</td><td>das Problem</td><td>the problem</td></tr>
        <tr><td>das Restaurant</td><td>the restaurant</td><td>das Regal</td><td>the shelf</td></tr>
        <tr><td>das Restaurant</td><td>the restaurant</td><td>das Rad</td><td>the wheel</td></tr>
        <tr><td>das Radio</td><td>the radio</td><td>das Schiff</td><td>the ship</td></tr>
        <tr><td>das Spiel</td><td>the game</td><td>das Stadion</td><td>the stadium</td></tr>
        <tr><td>das Stadtzentrum</td><td>the city center</td><td>das Theater</td><td>the theater</td></tr>
        <tr><td>das Tier</td><td>the animal</td><td>das Trinkwasser</td><td>the drinking water</td></tr>
        <tr><td>das Universum</td><td>the universe</td><td>das Urlaubsziel</td><td>the holiday destination</td></tr>
        <tr><td>das Verkehrsmittel</td><td>the means of transport</td><td>das Wetter</td><td>the weather</td></tr>
        <tr><td>das Zimmer</td><td>the room</td><td>das Zeichen</td><td>the sign/symbol</td></tr>
    </table>
</div>
</div>
</div>
        
        
        
        
</div>
</div>

<!-- Noun Plurals -->
<div id="plurals" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Noun Plurals</h1>
    
    <h2>1. Definition of Plural</h2>
    <p>A plural is used to refer to more than one person, animal, object, or concept. In German, plural forms vary by gender and noun endings.</p>
    <p>Examples:</p>
    <ul>
        <li>der Hund → die Hunde (the dog → the dogs)</li>
        <li>die Frau → die Frauen (the woman → the women)</li>
        <li>das Kind → die Kinder (the child → the children)</li>
    </ul>

    <!-- 2. Importance -->
    <h2>2. Importance</h2>
    <p>Plurals are essential for everyday conversation, shopping, asking questions, describing quantities, and grammar agreements with articles, adjectives, and verbs.</p>
    <ul>
        <li>Ich sehe <strong>die Kinder</strong> im Park. (I see the children in the park.)</li>
        <li>Die <strong>Frauen</strong> arbeiten im Büro. (The women work in the office.)</li>
        <li><strong>Die Hunde</strong> spielen im Garten. (The dogs are playing in the garden.)</li>
    </ul>

    <!-- 3. General Rules by Gender -->
    <h2>3. General Rules by Gender</h2>

    <!-- Masculine -->
    <h3>A. Masculine Nouns (der)</h3>
    <p>Common plural endings: -e, -er, -en, -n. Some nouns have umlaut changes (a → ä, o → ö, u → ü).</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>Rule/Pattern</th></tr>
        <tr><td>der Hund</td><td>die Hunde</td><td>add -e</td></tr>
        <tr><td>der Mann</td><td>die Männer</td><td>add -er + umlaut</td></tr>
        <tr><td>der Lehrer</td><td>die Lehrer</td><td>no change</td></tr>
        <tr><td>der Student</td><td>die Studenten</td><td>add -en</td></tr>
        <tr><td>der Vater</td><td>die Väter</td><td>umlaut + -er</td></tr>
    </table>
    <p>Example Sentences:</p>
    <ul>
        <li>Die <strong>Hunde</strong> bellen laut. (The dogs are barking loudly.)</li>
        <li>Meine <strong>Männer</strong> sind stark. (My men are strong.)</li>
    </ul>

    <!-- Feminine -->
    <h3>B. Feminine Nouns (die)</h3>
    <p>Common plural endings: -n, -en, -nen. Feminine nouns rarely change the stem vowel.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>Rule/Pattern</th></tr>
        <tr><td>die Frau</td><td>die Frauen</td><td>add -en</td></tr>
        <tr><td>die Lehrerin</td><td>die Lehrerinnen</td><td>add -innen</td></tr>
        <tr><td>die Lampe</td><td>die Lampen</td><td>add -n</td></tr>
        <tr><td>die Blume</td><td>die Blumen</td><td>add -n</td></tr>
        <tr><td>die Stadt</td><td>die Städte</td><td>umlaut + -e</td></tr>
    </table>
    <p>Example Sentences:</p>
    <ul>
        <li>Die <strong>Frauen</strong> sprechen miteinander. (The women are talking to each other.)</li>
        <li>Alle <strong>Lehrerinnen</strong> sind pünktlich. (All female teachers are on time.)</li>
    </ul>

    <!-- Neuter -->
    <h3>C. Neuter Nouns (das)</h3>
    <p>Common plural endings: -e, -er, -en, -s. Often includes umlaut changes.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>Rule/Pattern</th></tr>
        <tr><td>das Kind</td><td>die Kinder</td><td>add -er</td></tr>
        <tr><td>das Buch</td><td>die Bücher</td><td>umlaut + -er</td></tr>
        <tr><td>das Auto</td><td>die Autos</td><td>add -s</td></tr>
        <tr><td>das Haus</td><td>die Häuser</td><td>umlaut + -er</td></tr>
        <tr><td>das Fenster</td><td>die Fenster</td><td>no change</td></tr>
    </table>
    <p>Example Sentences:</p>
    <ul>
        <li>Die <strong>Kinder</strong> spielen im Garten. (The children are playing in the garden.)</li>
        <li>Ich habe zwei <strong>Bücher</strong> gekauft. (I bought two books.)</li>
    </ul>

    <!-- 4. Plural Formation Patterns -->
    <h2>4. Plural Formation Patterns</h2>
    <ul>
        <li>Masculine: often -e, -er, -en; sometimes umlaut</li>
        <li>Feminine: usually -n, -en; rarely umlaut</li>
        <li>Neuter: often -e, -er, -s; sometimes umlaut</li>
    </ul>
    <p>Examples:</p>
    <ul>
        <li>der Tisch → die Tische (table → tables)</li>
        <li>die Blume → die Blumen (flower → flowers)</li>
        <li>das Buch → die Bücher (book → books)</li>
    </ul>

    <!-- 5. Irregular Plurals -->
    <h2>5. Irregular Plurals</h2>
    <p>Some nouns are irregular and must be memorized:</p>
    <ul>
        <li>der Mann → die Männer</li>
        <li>das Kind → die Kinder</li>
        <li>die Mutter → die Mütter</li>
        <li>der Vater → die Väter</li>
        <li>die Stadt → die Städte</li>
    </ul>
    <p>Example Sentences:</p>
    <ul>
        <li>Die <strong>Männer</strong> arbeiten heute zu Hause. (The men are working from home today.)</li>
        <li>Ich sehe die <strong>Städte</strong> auf der Karte. (I see the cities on the map.)</li>
    </ul>

    <!-- 6. Noun Plurals with Articles -->
    <h2>6. Noun Plurals with Articles</h2>
    <p>Definite article: always <strong>die</strong> in plural. Indefinite article: there is no plural form.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th></tr>
        <tr><td>der Hund</td><td>die Hunde</td></tr>
        <tr><td>ein Hund</td><td>Hunde</td></tr>
        <tr><td>die Frau</td><td>die Frauen</td></tr>
        <tr><td>eine Frau</td><td>Frauen</td></tr>
        <tr><td>das Kind</td><td>die Kinder</td></tr>
        <tr><td>ein Kind</td><td>Kinder</td></tr>
    </table>
    <p>Example Sentences:</p>
    <ul>
        <li>Ich habe <strong>die Hunde</strong> gefüttert. (I fed the dogs.)</li>
        <li>Wir besuchen <strong>Frauen</strong> in der Stadt. (We visit women in the city.)</li>
    </ul>
<div id="plural-no-change">
    <h1>German Nouns with No Change in Plural</h1>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>Singular</th>
            <th>Plural</th>
            <th>Singular</th>
            <th>Plural</th>
        </tr>
        <tr><td>der Lehrer</td><td>die Lehrer</td><td>der Schüler</td><td>die Schüler</td></tr>
        <tr><td>der Arzt</td><td>die Ärzte</td><td>der Chef</td><td>die Chefs</td></tr>
        <tr><td>der Pilot</td><td>die Piloten</td><td>der Student</td><td>die Studenten</td></tr>
        <tr><td>der Präsident</td><td>die Präsidenten</td><td>der Ingenieur</td><td>die Ingenieure</td></tr>
        <tr><td>das Fenster</td><td>die Fenster</td><td>das Auto</td><td>die Autos</td></tr>
        <tr><td>das Hotel</td><td>die Hotels</td><td>das Café</td><td>die Cafés</td></tr>
        <tr><td>das Büro</td><td>die Büros</td><td>das Radio</td><td>die Radios</td></tr>
        <tr><td>das Restaurant</td><td>die Restaurants</td><td>das Kleid</td><td>die Kleider</td></tr>
        <tr><td>das Messer</td><td>die Messer</td><td>das Sofa</td><td>die Sofas</td></tr>
        <tr><td>das Telefon</td><td>die Telefone</td><td>das Fahrrad</td><td>die Fahrräder</td></tr>
        <tr><td>der Computer</td><td>die Computer</td><td>der Tisch</td><td>die Tische</td></tr>
        <tr><td>der Stuhl</td><td>die Stühle</td><td>der Schreibtisch</td><td>die Schreibtische</td></tr>
        <tr><td>der Laptop</td><td>die Laptops</td><td>der Koffer</td><td>die Koffer</td></tr>
        <tr><td>der Park</td><td>die Parks</td><td>der Garten</td><td>die Gärten</td></tr>
        <tr><td>der Zug</td><td>die Züge</td><td>der Bus</td><td>die Busse</td></tr>
        <tr><td>die Lampe</td><td>die Lampen</td><td>die Tasche</td><td>die Taschen</td></tr>
        <tr><td>die Blume</td><td>die Blumen</td><td>die Stadt</td><td>die Städte</td></tr>
        <tr><td>die Bank</td><td>die Banken</td><td>die Universität</td><td>die Universitäten</td></tr>
        <tr><td>die Schule</td><td>die Schulen</td><td>die Bibliothek</td><td>die Bibliotheken</td></tr>
        <tr><td>die Kirche</td><td>die Kirchen</td><td>die Stadtmitte</td><td>die Stadtmitten</td></tr>
        <tr><td>das Zimmer</td><td>die Zimmer</td><td>das Haus</td><td>die Häuser</td></tr>
        <tr><td>das Kind</td><td>die Kinder</td><td>das Buch</td><td>die Bücher</td></tr>
        <tr><td>das Heft</td><td>die Hefte</td><td>das Bild</td><td>die Bilder</td></tr>
        <tr><td>das Tier</td><td>die Tiere</td><td>das Jahr</td><td>die Jahre</td></tr>
        <tr><td>das Universum</td><td>die Universen</td><td>das Bürogebäude</td><td>die Bürogebäude</td></tr>
        <tr><td>das Museum</td><td>die Museen</td><td>das Stadion</td><td>die Stadien</td></tr>
        <tr><td>das Flugzeug</td><td>die Flugzeuge</td><td>das Schiff</td><td>die Schiffe</td></tr>
        <tr><td>das Kleidungsstück</td><td>die Kleidungsstücke</td><td>das Spielzeug</td><td>die Spielzeuge</td></tr>
    </table>
    
<div id="plural-add-s">
    <h1>German Nouns Plural by Adding -s</h1>
    <p>These nouns form their plural simply by adding <strong>-s</strong> at the end.</p>
    <ul>
        <li>das Auto → die Autos (car)</li>
        <li>das Café → die Cafés (café)</li>
        <li>das Hotel → die Hotels (hotel)</li>
        <li>das Radio → die Radios (radio)</li>
        <li>das Sofa → die Sofas (sofa)</li>
        <li>das Museum → die Museen (museum, exception with -en)</li>
        <li>das Handy → die Handys (mobile phone)</li>
        <li>das Taxi → die Taxis (taxi)</li>
        <li>das Baby → die Babys (baby)</li>
        <li>das Sandwich → die Sandwiches (sandwich)</li>
        <li>das Ticket → die Tickets (ticket)</li>
        <li>das Internet → die Internets (internet)**rare**</li>
        <li>das Video → die Videos (video)</li>
        <li>das Hobby → die Hobbys (hobby)</li>
        <li>das Restaurant → die Restaurants (restaurant)</li>
        <li>der Chef → die Chefs (boss)</li>
        <li>der Club → die Clubs (club)</li>
        <li>der Park → die Parks (park)</li>
        <li>der Laptop → die Laptops (laptop)</li>
        <li>der Job → die Jobs (job)</li>
        <li>der Tourist → die Tourists (tourist)</li>
        <li>der Student → die Students (student, informal sometimes)</li>
        <li>die Party → die Partys (party)</li>
        <li>die Show → die Shows (show)</li>
        <li>die SMS → die SMS (text message, no change, just plural article)</li>
        <li>die Cola → die Colas (cola)</li>
        <li>die Pizza → die Pizzas (pizza)</li>
        <li>die Banane → die Bananes (banana, borrowed form, sometimes -n)</li>
        <li>die Garage → die Garages (garage)</li>
        <li>die Idee → die Idees (idea, borrowed, less common)</li>
    </ul>
    
<div id="plural-umlaut-table">
    <h1>German Nouns Plural with Umlaut</h1>
    <p>These nouns form their plural by changing the vowel (umlaut) and sometimes adding -e or -er.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr>
            <th>Singular</th>
            <th>Plural</th>
            <th>Singular</th>
            <th>Plural</th>
        </tr>
        <tr><td>der Mann</td><td>die Männer</td><td>der Vater</td><td>die Väter</td></tr>
        <tr><td>der Sohn</td><td>die Söhne</td><td>der Bruder</td><td>die Brüder</td></tr>
        <tr><td>der Apfel</td><td>die Äpfel</td><td>der Stuhl</td><td>die Stühle</td></tr>
        <tr><td>der Fuß</td><td>die Füße</td><td>der Wald</td><td>die Wälder</td></tr>
        <tr><td>der Vogel</td><td>die Vögel</td><td>der Ofen</td><td>die Öfen</td></tr>
        <tr><td>der Nagel</td><td>die Nägel</td><td>der Hand</td><td>die Hände</td></tr>
        <tr><td>der Zahn</td><td>die Zähne</td><td>der Baum</td><td>die Bäume</td></tr>
        <tr><td>der Schuh</td><td>die Schuhe</td><td>der Tisch</td><td>die Tische</td></tr>
        <tr><td>der Käse</td><td>die Käse</td><td>der Name</td><td>die Namen</td></tr>
        <tr><td>der Fisch</td><td>die Fische</td><td>der Apfelbaum</td><td>die Apfelbäume</td></tr>
        <tr><td>der Vater</td><td>die Väter</td><td>der Sohn</td><td>die Söhne</td></tr>
        <tr><td>der Mann</td><td>die Männer</td><td>der Bruder</td><td>die Brüder</td></tr>
    </table>
<div id="must-know-plurals">
    <h1>Must-Know German Nouns – Plural Forms</h1>
    <p>Essential nouns for A1 learners with plural forms and English meanings.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>Singular</th><th>Plural</th></tr>
        <tr><td>der Apfel</td><td>die Äpfel</td><td>die Banane</td><td>die Bananen</td></tr>
        <tr><td>das Brot</td><td>die Brote</td><td>der Käse</td><td>die Käse</td></tr>
        <tr><td>die Milch</td><td>die Milch</td><td>das Wasser</td><td>die Wasser</td></tr>
        <tr><td>der Tee</td><td>die Tees</td><td>der Kaffee</td><td>die Kaffees</td></tr>
        <tr><td>die Butter</td><td>die Butter</td><td>das Ei</td><td>die Eier</td></tr>
        <tr><td>die Tomate</td><td>die Tomaten</td><td>der Salat</td><td>die Salate</td></tr>
        <tr><td>das Fleisch</td><td>die Fleisch</td><td>der Fisch</td><td>die Fische</td></tr>
        <tr><td>der Reis</td><td>die Reis</td><td>die Kartoffel</td><td>die Kartoffeln</td></tr>
        <tr><td>die Zwiebel</td><td>die Zwiebeln</td><td>der Zucker</td><td>die Zucker</td></tr>
        <tr><td>das Öl</td><td>die Öle</td><td>die Suppe</td><td>die Suppen</td></tr>
        <tr><td>der Teller</td><td>die Teller</td><td>das Glas</td><td>die Gläser</td></tr>
        <tr><td>der Löffel</td><td>die Löffel</td><td>die Gabel</td><td>die Gabeln</td></tr>
        <tr><td>das Messer</td><td>die Messer</td><td>der Topf</td><td>die Töpfe</td></tr>
        <tr><td>die Pfanne</td><td>die Pfannen</td><td>der Ofen</td><td>die Öfen</td></tr>
        <tr><td>der Kühlschrank</td><td>die Kühlschränke</td><td>die Mikrowelle</td><td>die Mikrowellen</td></tr>
        <tr><td>der Herd</td><td>die Herde</td><td>das Besteck</td><td>die Bestecke</td></tr>
        <tr><td>der Tisch</td><td>die Tische</td><td>der Stuhl</td><td>die Stühle</td></tr>
        <tr><td>das Buch</td><td>die Bücher</td><td>die Zeitung</td><td>die Zeitungen</td></tr>
        <tr><td>der Stift</td><td>die Stifte</td><td>das Heft</td><td>die Hefte</td></tr>
        <tr><td>der Rucksack</td><td>die Rucksäcke</td><td>die Tasche</td><td>die Taschen</td></tr>
        <tr><td>das Handy</td><td>die Handys</td><td>der Laptop</td><td>die Laptops</td></tr>
        <tr><td>das Telefon</td><td>die Telefone</td><td>die Uhr</td><td>die Uhren</td></tr>
        <tr><td>die Brille</td><td>die Brillen</td><td>der Schlüssel</td><td>die Schlüssel</td></tr>
        <tr><td>die Tür</td><td>die Türen</td><td>das Fenster</td><td>die Fenster</td></tr>
        <tr><td>die Wand</td><td>die Wände</td><td>der Boden</td><td>die Böden</td></tr>
        <tr><td>das Haus</td><td>die Häuser</td><td>die Wohnung</td><td>die Wohnungen</td></tr>
        <tr><td>die Straße</td><td>die Straßen</td><td>der Garten</td><td>die Gärten</td></tr>
        <tr><td>der Baum</td><td>die Bäume</td><td>die Blume</td><td>die Blumen</td></tr>
        <tr><td>das Tier</td><td>die Tiere</td><td>der Hund</td><td>die Hunde</td></tr>
        <tr><td>die Katze</td><td>die Katzen</td><td>das Pferd</td><td>die Pferde</td></tr>
        <tr><td>der Vogel</td><td>die Vögel</td><td>die Maus</td><td>die Mäuse</td></tr>
        <tr><td>der Fisch</td><td>die Fische</td><td>das Kaninchen</td><td>die Kaninchen</td></tr>
        <tr><td>die Schule</td><td>die Schulen</td><td>die Universität</td><td>die Universitäten</td></tr>
        <tr><td>der Lehrer</td><td>die Lehrer</td><td>die Lehrerin</td><td>die Lehrerinnen</td></tr>
        <tr><td>der Student</td><td>die Studenten</td><td>die Studentin</td><td>die Studentinnen</td></tr>
    </table>
</div>
</div>
</div>
    
    
</div>
    
    
    
    
</div>
</div>

<!-- Pronouns -->
<div id="pronouns" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Personal Pronouns</h1>
    
    <h2>1. Introduction & Definition</h2>
    <p>Personal pronouns are words that replace nouns referring to people, animals, or objects. They help avoid repetition and make sentences shorter and clearer.</p>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Anna ist müde. <strong>Sie</strong> schläft. (Anna is tired. She sleeps.)</li>
        <li>Der Hund läuft. <strong>Er</strong> ist schnell. (The dog runs. It is fast.)</li>
    </ul>

    <!-- 2. Subject Pronouns (Nominative) -->
    <h2>2. Subject Pronouns (Nominative)</h2>
    <p>Used as the subject of the sentence (who or what performs the action).</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>ich</td><td>wir</td><td>I / we</td></tr>
        <tr><td>du</td><td>ihr</td><td>you / you all (informal)</td></tr>
        <tr><td>er</td><td>sie</td><td>he / they</td></tr>
        <tr><td>sie</td><td>Sie</td><td>she / You (formal)</td></tr>
        <tr><td>es</td><td>-</td><td>it</td></tr>
    </table>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Ich lerne Deutsch. (I learn German.)</li>
        <li>Du bist mein Freund. (You are my friend.)</li>
        <li>Er spielt Fußball. (He plays soccer.)</li>
        <li>Wir gehen ins Kino. (We go to the cinema.)</li>
        <li>Sie sprechen Englisch. (They speak English.)</li>
        <li>Sie sind freundlich. (You [formal] are friendly.)</li>
    </ul>

    <!-- 3. Direct Object Pronouns (Accusative) -->
    <h2>3. Direct Object Pronouns (Accusative)</h2>
    <p>Used when the pronoun is the direct object of the sentence.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>mich</td><td>uns</td><td>me / us</td></tr>
        <tr><td>dich</td><td>euch</td><td>you / you all</td></tr>
        <tr><td>ihn</td><td>sie</td><td>him / them</td></tr>
        <tr><td>sie</td><td>Sie</td><td>her / You (formal)</td></tr>
        <tr><td>es</td><td>-</td><td>it</td></tr>
    </table>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Er sieht mich. (He sees me.)</li>
        <li>Ich liebe dich. (I love you.)</li>
        <li>Wir hören ihn. (We hear him.)</li>
        <li>Sie kennt uns. (She knows us.)</li>
        <li>Ich habe es gekauft. (I bought it.)</li>
    </ul>

    <!-- 4. Indirect Object Pronouns (Dative) -->
    <h2>4. Indirect Object Pronouns (Dative)</h2>
    <p>Used when the pronoun is the indirect object (to/for someone).</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>mir</td><td>uns</td><td>to/for me / us</td></tr>
        <tr><td>dir</td><td>euch</td><td>to/for you / you all</td></tr>
        <tr><td>ihm</td><td>ihnen</td><td>to/for him / them</td></tr>
        <tr><td>ihr</td><td>Ihnen</td><td>to/for her / You (formal)</td></tr>
        <tr><td>ihm</td><td>-</td><td>to/for it</td></tr>
    </table>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Er gibt mir das Buch. (He gives me the book.)</li>
        <li>Ich zeige dir die Stadt. (I show you the city.)</li>
        <li>Wir schenken ihm ein Geschenk. (We give him a gift.)</li>
        <li>Sie hilft ihnen. (She helps them.)</li>
        <li>Ich erkläre es ihr. (I explain it to her.)</li>
    </ul>

    <!-- 5. Reflexive Pronouns -->
    <h2>5. Reflexive Pronouns</h2>
    <p>Used when the subject and object are the same person.</p>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>mich</td><td>uns</td><td>myself / ourselves</td></tr>
        <tr><td>dich</td><td>euch</td><td>yourself / yourselves</td></tr>
        <tr><td>sich</td><td>sich</td><td>himself / herself / itself / themselves</td></tr>
    </table>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Ich wasche mich. (I wash myself.)</li>
        <li>Du setzt dich hin. (You sit down.)</li>
        <li>Er freut sich. (He is happy.)</li>
        <li>Wir treffen uns morgen. (We meet each other tomorrow.)</li>
        <li>Sie erinnern sich an das Lied. (They remember the song.)</li>
    </ul>

    <!-- 6. Verb Conjugation Agreement -->
    <h2>6. Verb Conjugation Agreement with Pronouns</h2>
    <p>The verb ending always depends on the subject pronoun.</p>
    <ul>
        <li>Ich <strong>bin</strong> müde. (I am tired.)</li>
        <li>Du <strong>bist</strong> nett. (You are kind.)</li>
        <li>Er <strong>hat</strong> ein Buch. (He has a book.)</li>
        <li>Wir <strong>gehen</strong> ins Kino. (We go to the cinema.)</li>
        <li>Sie <strong>sprechen</strong> Deutsch. (They speak German.)</li>
    </ul>
    <p><strong>Tip:</strong> For formal "Sie," always use the 3rd person plural form of the verb.</p>

    <!-- 7. Word Order with Pronouns -->
    <h2>7. Word Order with Pronouns</h2>
    <p>Pronouns usually come before nouns in a sentence. With modal verbs, they stay before the main verb.</p>
    <ul>
        <li>Ich gebe dir das Buch. (I give you the book.)</li>
        <li>Das Buch gebe ich dir. (I give you the book – emphasis on the book.)</li>
        <li>Er will mich sehen. (He wants to see me.)</li>
        <li>Wir können euch helfen. (We can help you all.)</li>
    </ul>

    <!-- 8. Common Mistakes & Tips -->
    <h2>8. Common Mistakes & Tips</h2>
    <ul>
        <li>Mixing informal and formal: du / Sie</li>
        <li>Confusing accusative vs dative pronouns</li>
        <li>For reflexive verbs, remember “sich” for 3rd person singular/plural</li>
        <li>Verb agreement is crucial: e.g., du <strong>bist</strong>, not du <strong>bin</strong></li>
    </ul
<div id="personal-pronoun-practice">
    <h1>Practice: Replacing Nouns with Personal Pronouns</h1>

    <!-- Paragraph 1: Original with nouns -->
    <h2>Original Paragraph (with Nouns)</h2>
    <p>
        Anna geht in die Schule. Peter spielt Fußball. Der Hund läuft im Garten. 
        Die Katze schläft auf dem Sofa. Ich sehe den Lehrer. Du hörst die Musik. 
        Maria kauft das Buch. Paul liest die Zeitung. Das Kind spielt im Park. 
        Die Eltern trinken Kaffee.
    </p>

    <!-- Paragraph 2: Replaced with personal pronouns -->
    <h2>Paragraph with Personal Pronouns</h2>
    <p>
        <u>Sie</u> geht in die Schule. <u>Er</u> spielt Fußball. <u>Er</u> läuft im Garten. 
        <u>Sie</u> schläft auf dem Sofa. <u>Ich</u> sehe <u>ihn</u>. <u>Du</u> hörst <u>sie</u>. 
        <u>Sie</u> kauft <u>es</u>. <u>Er</u> liest <u>sie</u>. <u>Es</u> spielt im Park. 
        <u>Sie</u> trinken Kaffee.
    </p>

    <!-- Explanation -->
    <h2>Explanation</h2>
    <p>
        In the second paragraph, the nouns were replaced by <strong>personal pronouns</strong> to make sentences shorter and easier to understand.  
        <ul>
            <li><u>Sie</u> replaces feminine nouns (Anna, die Katze, Maria).</li>
            <li><u>Er</u> replaces masculine nouns (Peter, der Hund, Paul).</li>
            <li><u>Es</u> replaces neuter nouns (das Kind, das Buch).</li>
            <li><u>Ich</u> and <u>Du</u> refer to the speaker and listener.</li>
            <li>Object nouns like den Lehrer, die Musik, das Buch, die Zeitung are replaced by <u>ihn</u>, <u>sie</u>, <u>es</u> in accusative.</li>
        </ul>
        This shows how personal pronouns simplify sentences while keeping the meaning intact.
    </p>
</div>
    
    

</div>
</div>

<!-- Negation -->
<div id="negation" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Basic Negation (kein/nicht)</h1>
    
    <h2>1. Introduction & Definition</h2>
    <p>Negation in German expresses “not” or “no.” It is used to indicate that something does not exist, is untrue, or is absent.</p>
    <p><strong>Examples:</strong></p>
    <ul>
        <li>Ich habe einen Hund. → Ich habe <strong>keinen</strong> Hund. (I have a dog → I have no dog.)</li>
        <li>Er spielt Fußball. → Er spielt <strong>nicht</strong> Fußball. (He plays soccer → He does not play soccer.)</li>
    </ul>

    <!-- 2. Negation with Kein -->
    <h2>2. Negation with "kein"</h2>
    <p>Used to negate nouns with indefinite articles (ein/eine) or without articles. Must agree with gender, number, and case.</p>
    
    <h3>Kein Table – Nominative</h3>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Gender</th><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>Masculine</td><td>kein</td><td>keine</td><td>no / not a</td></tr>
        <tr><td>Feminine</td><td>keine</td><td>keine</td><td>no / not a</td></tr>
        <tr><td>Neuter</td><td>kein</td><td>keine</td><td>no / not a</td></tr>
    </table>

    <h3>Kein Table – Accusative</h3>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Gender</th><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>Masculine</td><td>keinen</td><td>keine</td><td>no / not a</td></tr>
        <tr><td>Feminine</td><td>keine</td><td>keine</td><td>no / not a</td></tr>
        <tr><td>Neuter</td><td>kein</td><td>keine</td><td>no / not a</td></tr>
    </table>

    <h3>Kein Table – Dative</h3>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Gender</th><th>Singular</th><th>Plural</th><th>English</th></tr>
        <tr><td>Masculine</td><td>keinem</td><td>keinen</td><td>no / not a</td></tr>
        <tr><td>Feminine</td><td>keiner</td><td>keinen</td><td>no / not a</td></tr>
        <tr><td>Neuter</td><td>keinem</td><td>keinen</td><td>no / not a</td></tr>
    </table>

    <p><strong>Examples:</strong></p>
    <ul>
        <li>Ich habe <strong>keinen</strong> Hund. (I have no dog.)</li>
        <li>Sie trinkt <strong>keine</strong> Milch. (She drinks no milk.)</li>
        <li>Wir haben <strong>kein</strong> Auto. (We have no car.)</li>
        <li>Ich sehe <strong>keine</strong> Katzen. (I see no cats.)</li>
    </ul>

    <!-- 3. Negation with Nicht -->
    <h2>3. Negation with "nicht"</h2>
    <p>Used to negate verbs, adjectives, adverbs, prepositional phrases, or nouns with definite articles. Placement varies:</p>
    <ul>
        <li>Negating a verb: after the verb. Example: Ich spiele <strong>nicht</strong> Fußball.</li>
        <li>Negating an adjective or adverb: before the word. Example: Das Buch ist <strong>nicht</strong> interessant.</li>
        <li>Negating a prepositional phrase: before the phrase. Example: Er wohnt <strong>nicht</strong> in Berlin.</li>
    </ul>

    <!-- 4. Differences between Kein & Nicht -->
    <h2>4. Differences between "kein" and "nicht"</h2>
    <table border="1" cellpadding="5" cellspacing="0">
        <tr><th>Usage</th><th>Example</th><th>Explanation</th></tr>
        <tr><td>kein</td><td>Ich habe <strong>keinen</strong> Stift.</td><td>Negates nouns with indefinite article or no article.</td></tr>
        <tr><td>nicht</td><td>Ich habe den Stift <strong>nicht</strong>.</td><td>Negates verbs, adjectives, adverbs, prepositional phrases, or nouns with definite article.</td></tr>
    </table>

    <p><strong>Tip:</strong> Use <strong>kein</strong> for “no…” or “I have no…”, and <strong>nicht</strong> to negate actions, descriptions, or phrases.</p>

    <!-- 5. Common Mistakes -->
    <h2>5. Common Mistakes</h2>
    <ul>
        <li>❌ Ich habe nicht Hund. → ✅ Ich habe <strong>keinen</strong> Hund.</li>
        <li>❌ Ich trinke kein die Milch. → ✅ Ich trinke <strong>nicht</strong> die Milch.</li>
        <li>Placement of <strong>nicht</strong> before the wrong word is incorrect.</li>
    </ul>

    <!-- 6. Vocabulary Examples -->
    <h2>6. Vocabulary Examples</h2>
    <p>Common nouns for <strong>kein</strong>: Hund, Auto, Buch, Milch, Geld, Katze, Haus, Stuhl, Ball, Schule</p>
    <p>Common verbs/adjectives/adverbs for <strong>nicht</strong>: gehen, spielen, groß, klein, interessant, schnell, heute, morgen, müde, schön</p>

    <!-- 7. Combined Sentences -->
    <h2>7. Combined Sentences with Kein & Nicht</h2>
    <ul>
        <li>Ich habe <strong>kein</strong> Auto und fahre <strong>nicht</strong> mit dem Bus.</li>
        <li>Sie trinkt <strong>keinen</strong> Kaffee, aber sie isst Kuchen <strong>nicht</strong>.</li>
    </ul>

    <!-- 8. Mini Practice Sentences -->
    <h2>8. Mini Practice</h2>
    <ol>
        <li>Ich habe _____ Buch. (kein / nicht)</li>
        <li>Er spielt _____ Tennis. (kein / nicht)</li>
        <li>Wir haben _____ Geld. (kein / nicht)</li>
        <li>Die Katze schläft _____ auf dem Sofa. (kein / nicht)</li>
        <li>Du trinkst _____ Kaffee. (kein / nicht)</li>
    </ol>

    <!-- 9. Paragraph Examples -->
    <h2>9. Paragraph Example</h2>
    <p>
        Heute habe ich <strong>kein</strong> Auto. Ich gehe <strong>nicht</strong> mit dem Bus. 
        Mein Bruder hat <strong>kein</strong> Fahrrad, er fährt <strong>nicht</strong> zur Schule. 
        Meine Eltern trinken <strong>keinen</strong> Kaffee, sie trinken Tee <strong>nicht</strong>. 
        Die Katze spielt <strong>nicht</strong> im Garten, sie schläft. 
        Ich sehe <strong>keine</strong> Vögel draußen.
    </p>

    <!-- 10. Explanation -->
    <h2>10. Explanation</h2>
    <p>
        - <strong>Kein</strong> replaces nouns with indefinite articles or no article.  
        - <strong>Nicht</strong> negates verbs, adjectives, adverbs, prepositional phrases, or nouns with definite articles.  
        - Placement of <strong>nicht</strong> is important: always before the word or phrase you want to negate.  
        - Use these rules to make correct negative sentences in German.
    </p>
<div id="mixed-kein-nicht-examples">
    <h1>Practice: Mixed "Kein" and "Nicht"</h1>

    <h2>20 Sentences from Simple to Complex</h2>
    <ol>
        <li>Ich habe <strong>kein</strong> Buch. (I have no book.)</li>
        <li>Er spielt <strong>nicht</strong> Fußball. (He does not play soccer.)</li>
        <li>Das Haus ist <strong>nicht</strong> groß. (The house is not big.)</li>
        <li>Ich trinke <strong>keinen</strong> Kaffee. (I drink no coffee.)</li>
        <li>Wir haben <strong>kein</strong> Auto und gehen zu Fuß. (We have no car and go on foot.)</li>
        <li>Sie spielt heute <strong>nicht</strong> Tennis. (She does not play tennis today.)</li>
        <li>Ich habe <strong>keinen</strong> Hund und er spielt <strong>nicht</strong> im Garten. (I have no dog and he does not play in the garden.)</li>
        <li>Meine Eltern trinken <strong>keinen</strong> Kaffee, aber sie essen Kuchen <strong>nicht</strong>. (My parents drink no coffee, but they do not eat cake.)</li>
        <li>Ich habe <strong>kein</strong> Geld, deshalb kaufe ich das Buch <strong>nicht</strong>. (I have no money, therefore I do not buy the book.)</li>
        <li>Er hat <strong>keinen</strong> Stift, und er kann den Brief <strong>nicht</strong> schreiben. (He has no pen, and he cannot write the letter.)</li>
        <li>Du hast <strong>keine</strong> Idee, und das ist <strong>nicht</strong> gut. (You have no idea, and that is not good.)</li>
        <li>Wir sehen <strong>keine</strong> Vögel, und der Hund schläft <strong>nicht</strong>. (We see no birds, and the dog does not sleep.)</li>
        <li>Ich esse <strong>keine</strong> Äpfel, aber ich trinke Saft <strong>nicht</strong>. (I eat no apples, but I do not drink juice.)</li>
        <li>Sie hat <strong>keinen</strong> Bruder, und ihre Schwester spricht <strong>nicht</strong> Englisch. (She has no brother, and her sister does not speak English.)</li>
        <li>Das Kind hat <strong>kein</strong> Spielzeug, und es spielt <strong>nicht</strong> draußen. (The child has no toy, and it does not play outside.)</li>
        <li>Wir haben <strong>keine</strong> Zeit, und wir können heute <strong>nicht</strong> kommen. (We have no time, and we cannot come today.)</li>
        <li>Ich sehe <strong>keine</strong> Katze, und der Hund bellt <strong>nicht</strong>. (I see no cat, and the dog does not bark.)</li>
        <li>Er trinkt <strong>keinen</strong> Tee, und ich esse Kuchen <strong>nicht</strong>. (He drinks no tea, and I do not eat cake.)</li>
        <li>Sie hat <strong>kein</strong> Handy, und sie telefoniert <strong>nicht</strong>. (She has no phone, and she does not make calls.)</li>
        <li>Wir besitzen <strong>keine</strong> Bücher, und wir lesen <strong>nicht</strong>. (We own no books, and we do not read.)</li>
    </ol>

    <h2>Explanation</h2>
    <p>
        - <strong>Kein</strong> is used to negate nouns with indefinite articles or without articles.  
        - <strong>Nicht</strong> is used to negate verbs, adjectives, adverbs, prepositional phrases, or nouns with definite articles.  
        - In sentences with both <strong>kein</strong> and <strong>nicht</strong>, <strong>kein</strong> usually negates the noun first, and <strong>nicht</strong> negates the action, description, or phrase.  
    </p>
</div>
    
    
</div>
</div>

<!-- Modal Verbs -->
<div id="modal" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Modal Verbs Basics</h1>
    
    <h2>1. Introduction & Definition</h2>
    <p>Modal verbs are verbs that <strong>change the meaning of the main verb</strong> in a sentence. They express <strong>ability, necessity, permission, desire, or obligation</strong>.</p>
    <p>The most common A1 modal verbs are:</p>
    <ul>
        <li><strong>können</strong> – can / to be able to</li>
        <li><strong>müssen</strong> – must / have to</li>
        <li><strong>dürfen</strong> – may / allowed to</li>
        <li><strong>wollen</strong> – want to</li>
        <li><strong>sollen</strong> – should / supposed to</li>
        <li><strong>mögen</strong> – like to</li>
    </ul>

    <h3>Examples:</h3>
    <ul>
        <li>Ich <strong>kann</strong> Deutsch sprechen. (I can speak German.)</li>
        <li>Du <strong>musst</strong> Hausaufgaben machen. (You must do homework.)</li>
        <li>Er <strong>darf</strong> heute schwimmen. (He may swim today.)</li>
        <li>Wir <strong>wollen</strong> ins Kino gehen. (We want to go to the cinema.)</li>
    </ul>

    <!-- 2. Conjugation of "können" -->
    <h2>2. Conjugation of a Modal Verb – "können"</h2>
    <p>Present tense conjugation of <strong>können</strong>:</p>
    <ul>
        <li>ich <strong>kann</strong></li>
        <li>du <strong>kannst</strong></li>
        <li>er/sie/es <strong>kann</strong></li>
        <li>wir <strong>können</strong></li>
        <li>ihr <strong>könnt</strong></li>
        <li>sie/Sie <strong>können</strong></li>
    </ul>

    <h3>Examples with "können":</h3>
    <ul>
        <li>Ich <strong>kann</strong> schwimmen.</li>
        <li>Du <strong>kannst</strong> Fußball spielen.</li>
        <li>Wir <strong>können</strong> Deutsch lernen.</li>
        <li>Sie <strong>können</strong> heute nicht kommen.</li>
    </ul>

    <p>Other modal verbs (<strong>müssen, dürfen, wollen, sollen, mögen</strong>) follow the <strong>same pattern</strong> but with their own stem.</p>
    <h3>Examples with other modal verbs:</h3>
    <ul>
        <li>Ich <strong>muss</strong> früh aufstehen.</li>
        <li>Du <strong>darfst</strong> ins Kino gehen.</li>
        <li>Wir <strong>wollen</strong> einen Film sehen.</li>
        <li>Sie <strong>sollen</strong> leise sein.</li>
    </ul>

    <!-- 3. Basic Sentence Structure -->
    <h2>3. Basic Sentence Structure</h2>
    <p>Structure: <strong>Subject + Modal Verb + Main Verb (Infinitive at the end)</strong></p>
    <ul>
        <li>Ich <strong>kann</strong> Deutsch sprechen.</li>
        <li>Du <strong>musst</strong> die Hausaufgaben machen.</li>
        <li>Er <strong>darf</strong> heute Fußball spielen.</li>
        <li>Wir <strong>wollen</strong> morgen ins Kino gehen.</li>
    </ul>

    <h3>Negation with "nicht":</h3>
    <ul>
        <li>Ich <strong>kann nicht</strong> singen.</li>
        <li>Du <strong>darfst nicht</strong> rauchen.</li>
        <li>Wir <strong>wollen nicht</strong> früh aufstehen.</li>
        <li>Sie <strong>mögen nicht</strong> Kaffee trinken.</li>
    </ul>

    <!-- 4. Expressing Ability / Permission / Obligation / Desire -->
    <h2>4. Expressing Ability / Permission / Obligation / Desire</h2>
    
    <h3>Ability – "können"</h3>
    <ul>
        <li>Ich <strong>kann</strong> jeden Tag Deutsch lernen.</li>
        <li>Du <strong>kannst</strong> gut tanzen.</li>
        <li>Er <strong>kann</strong> das Problem lösen.</li>
        <li>Wir <strong>können</strong> gut singen.</li>
    </ul>

    <h3>Necessity / Obligation – "müssen / sollen"</h3>
    <ul>
        <li>Ich <strong>muss</strong> meine Hausaufgaben machen.</li>
        <li>Du <strong>sollst</strong> gesund essen.</li>
        <li>Er <strong>muss</strong> früh aufstehen.</li>
        <li>Wir <strong>sollen</strong> pünktlich sein.</li>
    </ul>

    <h3>Permission – "dürfen"</h3>
    <ul>
        <li>Ich <strong>darf</strong> heute später kommen.</li>
        <li>Du <strong>darfst</strong> das Buch lesen.</li>
        <li>Sie <strong>darf</strong> ins Kino gehen.</li>
        <li>Wir <strong>dürfen</strong> hier nicht rauchen.</li>
    </ul>

    <h3>Desire / Want – "wollen / mögen"</h3>
    <ul>
        <li>Ich <strong>will</strong> ins Kino gehen.</li>
        <li>Du <strong>willst</strong> Schokolade essen.</li>
        <li>Wir <strong>mögen</strong> Fußball spielen.</li>
        <li>Sie <strong>mögen</strong> Tee trinken.</li>
    </ul>

    <!-- 5. Questions with Modal Verbs -->
    <h2>5. Questions with Modal Verbs</h2>

    <h3>Yes / No questions:</h3>
    <ul>
        <li><strong>Kann</strong> ich Deutsch sprechen?</li>
        <li><strong>Musst</strong> du heute arbeiten?</li>
        <li><strong>Darf</strong> er ins Kino gehen?</li>
        <li><strong>Wollen</strong> wir Pizza essen?</li>
    </ul>

    <h3>W-questions:</h3>
    <ul>
        <li><strong>Was kann</strong> ich tun?</li>
        <li><strong>Wann musst</strong> du zur Schule gehen?</li>
        <li><strong>Warum darf</strong> er nicht kommen?</li>
        <li><strong>Wo wollen</strong> wir essen gehen?</li>
    </ul>

    <!-- 6. Practice Exercises -->
    <h2>6. Practice Exercises</h2>
    <p>Fill in the blanks with the correct modal verb (können, müssen, dürfen, wollen, sollen, mögen):</p>
    <ol>
        <li>Ich _____ Deutsch sprechen. (können / müssen)</li>
        <li>Du _____ Hausaufgaben machen. (dürfen / müssen)</li>
        <li>Er _____ ins Kino gehen. (wollen / mögen)</li>
        <li>Wir _____ pünktlich sein. (sollen / können)</li>
        <li>Sie _____ Schokolade essen. (mögen / dürfen)</li>
        <li>Ich _____ nicht singen. (kann / will)</li>
        <li>Du _____ nicht rauchen. (darfst / musst)</li>
        <li>Wir _____ früh aufstehen. (müssen / wollen)</li>
        <li>Er _____ das Problem lösen. (kann / soll)</li>
        <li>Sie _____ Tee trinken. (mögen / müssen)</li>
    </ol>

    <!-- 7. Short Paragraph with Modal Verbs -->
    <h2>7. Short Paragraph</h2>
    <p>
        Ich <strong>kann</strong> jeden Tag Deutsch lernen.<br>
        Du <strong>musst</strong> früh aufstehen.<br>
        Er <strong>darf</strong> heute Fußball spielen.<br>
        Wir <strong>wollen</strong> ins Kino gehen.<br>
        Ihr <strong>sollt</strong> leise sein.<br>
        Sie <strong>mögen</strong> Musik hören.<br>
        Ich <strong>kann nicht</strong> singen, aber ich <strong>will</strong> Gitarre spielen.
    </p>
<div id="modal-verbs-paragraph">
    <h1>Observe Modal Verb Changes in Daily Life Activities</h1>

    <p>
        Ich <u>muss</u> jeden Morgen früh aufstehen, um pünktlich zur Arbeit zu gehen.<br>
        Meine Schwester <u>will</u> heute Kuchen backen, aber sie <u>darf</u> die Küche nicht alleine benutzen.<br>
        Wir <u>können</u> zusammen nach der Schule spazieren gehen.<br>
        Mein Bruder <u>möchte</u> Fußball spielen, aber er <u>soll</u> zuerst seine Hausaufgaben machen.<br>
        <u>Kannst</u> du mir helfen, die Blumen zu gießen? (Question)<br>
        Ich <u>mag</u> Kaffee trinken, aber heute <u>mag</u> ich lieber Tee.<br>
        Wir <u>dürfen</u> am Wochenende länger schlafen.<br>
        Ihr <u>sollt</u> leise sein, weil die Nachbarn schlafen.<br>
        Trotzdem <u>können</u> wir am Nachmittag im Garten spielen.<br>
        Meine Eltern fragen: „<u>Müssen</u> wir wirklich so früh aufstehen?“ (Question)<br>
        Ich <u>will</u> die Zeitung lesen, aber ich <u>kann</u> sie nicht finden.<br>
        Am Abend <u>möchten</u> wir einen Film sehen, und wir <u>dürfen</u> die Couch benutzen.
    </p>

    <h2>English Translation</h2>
    <p>
        I <u>must</u> get up early every morning to be on time for work.<br>
        My sister <u>wants</u> to bake a cake today, but she <u>may</u> not use the kitchen alone.<br>
        We <u>can</u> go for a walk together after school.<br>
        My brother <u>wants</u> to play football, but he <u>should</u> do his homework first.<br>
        <u>Can</u> you help me water the flowers? (Question)<br>
        I <u>like</u> to drink coffee, but today I <u>prefer</u> tea.<br>
        We <u>are allowed</u> to sleep longer on weekends.<br>
        You (plural) <u>should</u> be quiet because the neighbors are sleeping.<br>
        Nevertheless, we <u>can</u> play in the garden in the afternoon.<br>
        My parents ask: "<u>Do we have to</u> get up so early?" (Question)<br>
        I <u>want</u> to read the newspaper, but I <u>cannot</u> find it.<br>
        In the evening, we <u>want</u> to watch a movie, and we <u>are allowed</u> to use the couch.
    </p>

    <h2>Observation:</h2>
    <ul>
        <li>Each modal verb changes its form according to the **subject** (ich, du, er/sie/es, wir, ihr, sie/Sie).</li>
        <li>Questions move the **modal verb to the beginning** of the sentence.</li>
        <li>Negation with <strong>nicht</strong> is used to show inability or prohibition.</li>
        <li>The **main verb** always stays at the end in its **infinitive form**.</li>
    </ul>
</div>

    <!-- 8. Explanation -->
    <h2>8. Explanation for Learners</h2>
    <p>
        - Modal verbs modify the main verb to express ability, necessity, permission, desire, or obligation.<br>
        - The <strong>main verb always goes to the end</strong> in infinitive form.<br>
        - Other modal verbs follow the same conjugation pattern as <strong>können</strong>.<br>
        - Use <strong>nicht</strong> to negate modal verbs or the main verb.<br>
        - Questions invert the subject and the modal verb.
    </p>
</div>
</div>

<!-- Word Order -->
<div id="wordOrder" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Word Order in Main Clause</h1>
    

<h2>1. Definition</h2>
<p>A <strong>main clause</strong> (<em>Hauptsatz</em>) is a sentence that can stand alone. The finite verb always comes second (V2 rule). This ensures the sentence is grammatically correct and understandable.</p>
<p><strong>How it works:</strong> The first position is flexible for emphasis (time, place, subject, object), but the verb must always occupy the second position.</p>
<ul>
<li>Ich <strong>gehe</strong> nach Hause. – Verb second, subject first.</li>
<li>Heute <strong>gehe</strong> ich nach Hause. – Time first, verb second.</li>
<li>Nach Hause <strong>gehe</strong> ich heute. – Place first for style.</li>
<li>Mein Bruder <strong>spielt</strong> Fußball. – Normal subject-verb order.</li>
<li>Morgen <strong>kommt</strong> meine Freundin zu Besuch. – Time first, verb second, subject after verb.</li>
</ul>

<h2>2. General Structure</h2>
<p>Standard structure: <strong>[First element] + Finite Verb + [Other elements]</strong>.</p>
<ul>
<li>Ich <strong>lese</strong> ein Buch. – Subject first, object last.</li>
<li>Heute <strong>essen</strong> wir Pizza. – Time first, subject after verb.</li>
<li>Das Kind <strong>schläft</strong> tief. – Subject first, adverb last.</li>
<li>Meine Eltern <strong>fahren</strong> nach Berlin. – Simple order.</li>
<li>Morgen <strong>beginnt</strong> die Schule wieder. – Time first, verb second.</li>
</ul>

<h2>3. Time – Manner – Place (TMP) Rule</h2>
<p>After the verb, the typical order is: <strong>Time → Manner → Place</strong>.</p>
<ul>
<li>Ich <strong>gehe</strong> heute mit meinen Freunden ins Kino.</li>
<li>Er <strong>arbeitet</strong> morgen sehr fleißig in der Bibliothek.</li>
<li>Wir <strong>fahren</strong> nächste Woche mit dem Zug nach München.</li>
<li>Sie <strong>tanzt</strong> jeden Samstag voller Freude im Club.</li>
<li>Du <strong>kommst</strong> heute Abend pünktlich zum Konzert.</li>
</ul>

<h2>4. Objects (Accusative & Dative)</h2>
<p>Indirect (dative) objects often come before direct (accusative) objects. Pronouns usually precede nouns.</p>
<ul>
<li>Ich <strong>gebe</strong> dem Mann das Buch.</li>
<li>Sie <strong>schreibt</strong> ihrer Freundin einen Brief.</li>
<li>Wir <strong>zeigen</strong> den Touristen die Stadt.</li>
<li>Er <strong>kauft</strong> seiner Schwester einen Pullover.</li>
<li>Du <strong>bringst</strong> dem Lehrer die Hausaufgaben.</li>
</ul>
<p><strong>Pronouns before nouns:</strong></p>
<ul>
<li>Ich <strong>gebe ihm</strong> das Buch.</li>
<li>Sie <strong>schickt ihr</strong> einen Brief.</li>
<li>Wir <strong>zeigen ihnen</strong> die Stadt.</li>
<li>Du <strong>kaufst ihr</strong> einen Blumenstrauß.</li>
<li>Er <strong>bringt ihm</strong> das Essen.</li>
</ul>

<h2>5. Negation</h2>
<p>Placement of <strong>nicht</strong> depends on what is negated, either before the element or at the end.</p>
<ul>
<li>Ich <strong>sehe</strong> den Film <strong>nicht</strong>.</li>
<li>Heute <strong>gehe</strong> ich <strong>nicht</strong> ins Kino.</li>
<li>Sie <strong>ist</strong> <strong>nicht</strong> müde.</li>
<li>Wir <strong>haben</strong> das Buch <strong>nicht</strong> gelesen.</li>
<li>Er <strong>trinkt</strong> <strong>nie</strong> Kaffee.</li>
</ul>

<h2>6. Modal and Auxiliary Verbs</h2>
<ul>
<li>Ich <strong>kann</strong> heute nicht kommen.</li>
<li>Wir <strong>haben</strong> das Buch gelesen.</li>
<li>Sie <strong>möchte</strong> ein Eis essen.</li>
<li>Er <strong>soll</strong> mehr lernen.</li>
<li>Ihr <strong>dürft</strong> hier nicht parken.</li>
</ul>

<h2>7. Compound Tenses / Multiple Verbs</h2>
<ul>
<li>Ich <strong>habe</strong> das Buch gelesen.</li>
<li>Er <strong>wird</strong> morgen nach Berlin fahren.</li>
<li>Sie <strong>hat</strong> das Buch nicht lesen können.</li>
<li>Wir <strong>werden</strong> bald ein neues Auto kaufen.</li>
<li>Du <strong>hast</strong> gestern sehr gut geschlafen.</li>
</ul>

<h2>8. Conjunctions</h2>
<h3>a) Coordinating</h3>
<ul>
<li>Ich gehe ins Kino, <strong>aber</strong> er bleibt zu Hause.</li>
<li>Wir fahren nach München, <strong>und</strong> sie kommen mit.</li>
<li>Du kannst Tee trinken, <strong>oder</strong> du nimmst Wasser.</li>
<li>Er arbeitet viel, <strong>denn</strong> er möchte Geld sparen.</li>
<li>Ich mag Schokolade, <strong>aber</strong> ich esse sie selten.</li>
</ul>
<h3>b) Subordinating</h3>
<ul>
<li>Ich bleibe zu Hause, <strong>weil</strong> ich müde bin.</li>
<li>Er sagt, <strong>dass</strong> er später kommt.</li>
<li>Wir gehen nicht schwimmen, <strong>obwohl</strong> es warm ist.</li>
<li>Sie freut sich, <strong>weil</strong> sie gute Noten bekommen hat.</li>
<li>Ich glaube, <strong>dass</strong> das Wetter schön wird.</li>
</ul>

<h2>9. Advanced Sentence Structures</h2>
<p>Higher-level structures include inversion, emphasis, complex objects, and multiple verbs. These make sentences more fluent and natural.</p>

<h3>1. Inversion (questions)</h3>
<ul>
<li><strong>Geht</strong> er heute ins Kino?</li>
<li><strong>Hast</strong> du das Buch gelesen?</li>
<li><strong>Kommt</strong> sie morgen zur Party?</li>
<li><strong>Kann</strong> ich hier sitzen?</li>
<li><strong>Wird</strong> er pünktlich sein?</li>
</ul>

<h3>2. Emphasis / Stylistic first element</h3>
<ul>
<li><strong>Dieses Buch</strong> lese ich morgen.</li>
<li><strong>Heute Abend</strong> essen wir Pizza.</li>
<li><strong>Die Hausaufgaben</strong> mache ich später.</li>
<li><strong>Im Garten</strong> spielt das Kind.</li>
<li><strong>Morgen</strong> fahre ich nach Berlin.</li>
</ul>

<h3>3. Multiple verbs / complex tenses</h3>
<ul>
<li>Sie <strong>hat</strong> das Buch nicht lesen können.</li>
<li>Wir <strong>werden</strong> morgen einkaufen gehen.</li>
<li>Ich <strong>habe</strong> das Auto reparieren lassen.</li>
<li>Er <strong>wird</strong> bald nach Hause zurückkehren.</li>
<li>Du <strong>hast</strong> das Problem nicht lösen können.</li>
</ul>

<h3>4. Complex objects / subordinate clauses</h3>
<ul>
<li>Ich <strong>erwarte</strong>, dass du pünktlich bist.</li>
<li>Er <strong>weiß</strong>, dass sie nach Berlin fährt.</li>
<li>Wir <strong>hoffen</strong>, dass alles gut geht.</li>
<li>Sie <strong>glaubt</strong>, dass er recht hat.</li>
<li>Ich <strong>denke</strong>, dass du das verstehen wirst.</li>
</ul>

<h3>5. Negation with multiple verbs</h3>
<ul>
<li>Ich <strong>habe</strong> das Buch nicht lesen können.</li>
<li>Er <strong>wird</strong> das Problem nicht lösen können.</li>
<li>Wir <strong>haben</strong> den Fehler nicht bemerkt.</li>
<li>Sie <strong>möchte</strong> das Geschenk nicht annehmen.</li>
<li>Du <strong>kannst</strong> das nicht verstehen.</li>
</ul>

<h2>10. Summary Table – Main Clause Word Order</h2>
<table border="1">
<tr>
<th>Element</th>
<th>Position</th>
<th>Examples</th>
</tr>
<tr>
<td>Subject / First Element</td>
<td>1st</td>
<td>Ich / Heute / Das Buch / Morgen / Im Garten</td>
</tr>
<tr>
<td>Finite Verb</td>
<td>2nd</td>
<td>gehe / spielt / liest / fährt / kommt</td>
</tr>
<tr>
<td>Time</td>
<td>After verb</td>
<td>heute, morgen, nächste Woche, jeden Samstag, heute Abend</td>
</tr>
<tr>
<td>Manner</td>
<td>After time</td>
<td>mit Freunden, sehr fleißig, voller Freude, pünktlich, langsam</td>
</tr>
<tr>
<td>Place</td>
<td>After manner</td>
<td>ins Kino, in der Bibliothek, nach München, im Club, nach Hause</td>
</tr>
<tr>
<td>Objects</td>
<td>After verb/adverbs</td>
<td>dem Mann das Buch, ihrer Freundin einen Brief, den Touristen die Stadt, seiner Schwester einen Pullover, dem Lehrer die Hausaufgaben</td>
</tr>
<tr>
<td>Infinitive (modal/aux)</td>
<td>End</td>
<td>nach Hause gehen, lesen, kaufen, fahren, schlafen</td>
</tr>
<tr>
<td>Negation</td>
<td>Before element / end</td>
<td>nicht, nie, kein, nie wieder, kein Problem</td>
</tr>
</table>

</html>
</div>

<!-- Questions -->
<div id="questions" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Yes/No & W-Questions</h1>
    

<h2>1. Yes/No Questions (Ja/Nein Fragen)</h2>

<h3>1.1 Definition</h3>
<p>Yes/No questions can be answered with <strong>Ja</strong> or <strong>Nein</strong>. The verb comes first in German.</p>

<h3>1.2 Basic Structure</h3>
<p>Verb + Subject + Rest</p>

<h3>1.3 Basic Examples</h3>
<p>
Bist du müde? → Are you tired?<br>
Hast du Hunger? → Do you have hunger?<br>
Kommst du morgen? → Are you coming tomorrow?<br>
Spielst du Fußball? → Do you play football?<br>
Geht er zur Schule? → Is he going to school?
</p>

<h3>1.4 Modal Verbs in Yes/No Questions</h3>
<p>Structure: Modal verb + Subject + Main verb (infinitive)</p>
<p>
Kannst du schwimmen? → Can you swim?<br>
Willst du nach Hause gehen? → Do you want to go home?<br>
Musst du heute arbeiten? → Do you have to work today?<br>
Darf ich hier sitzen? → May I sit here?<br>
Sollen wir anfangen? → Should we start?
</p>

<h3>1.5 Tense Variations</h3>

<p><strong>Perfect (Perfekt):</strong> Auxiliary (haben/sein) + Subject + Past Participle + Rest</p>
<p>
Hast du das Buch gelesen? → Did you read the book?<br>
Bist du gestern nach Hause gegangen? → Did you go home yesterday?<br>
Habt ihr schon gegessen? → Have you already eaten?
</p>

<p><strong>Simple Past (Präteritum):</strong> Verb (past) + Subject + Rest</p>
<p>
Hattest du Zeit? → Did you have time?<br>
Warst du krank? → Were you sick?<br>
Spielte er gestern Fußball? → Did he play football yesterday?
</p>

<h3>1.6 Advanced Yes/No Questions</h3>

<p><strong>a) With Subordinate Clauses:</strong><br>
Glaubst du, dass er kommt? → Do you believe he is coming?<br>
Meinst du, dass sie die Prüfung bestanden hat? → Do you think she passed the exam?<br>
Denkst du, dass wir pünktlich sind? → Do you think we are on time?<br>
Hoffst du, dass er morgen kommt? → Do you hope he will come tomorrow?
</p>

<p><strong>b) Separable Verbs:</strong><br>
Stehst du früh auf? → Do you get up early?<br>
Rufst du mich morgen an? → Will you call me tomorrow?<br>
Bringst du das Buch mit? → Are you bringing the book along?<br>
Fängst du spät an? → Are you starting late?
</p>

<p><strong>c) Negation:</strong><br>
Kommst du nicht morgen? → Aren’t you coming tomorrow?<br>
Hast du kein Geld? → Don’t you have any money?<br>
Willst du nicht mitkommen? → Don’t you want to come along?<br>
Kann er nicht schwimmen? → Can’t he swim?
</p>

<p><strong>d) Polite/Formal:</strong><br>
Haben Sie Zeit? → Do you have time?<br>
Können Sie mir helfen? → Can you help me?<br>
Waren Sie schon einmal in Berlin? → Have you ever been to Berlin?<br>
Dürfen wir hier sitzen? → May we sit here?
</p>

<p><strong>Extra Advanced Examples:</strong><br>
Hast du das Problem schon gelöst? → Have you already solved the problem?<br>
Bist du jemals nach Deutschland gereist? → Have you ever traveled to Germany?<br>
Können wir morgen beginnen? → Can we start tomorrow?<br>
Willst du das wirklich tun? → Do you really want to do that?<br>
Darf ich fragen? → May I ask?
</p>

<hr>

<h2>2. WH-Questions (W-Fragen)</h2>

<h3>2.1 Definition</h3>
<p>Questions starting with a question word to get information beyond Yes/No. Structure: Question word + Verb + Subject + Rest</p>

<h3>2.2 Question Words List</h3>
<p>
Wer → Who<br>
Was → What<br>
Wo → Where<br>
Wohin → Where to<br>
Woher → Where from<br>
Wann → When<br>
Warum → Why<br>
Wie → How<br>
Wieviel / Wie viele → How much / How many<br>
Welcher/Welche/Welches → Which
</p>

<h3>2.3 Basic Examples</h3>
<p>
Wer kommt morgen? → Who is coming tomorrow?<br>
Was machst du? → What are you doing?<br>
Wo wohnst du? → Where do you live?<br>
Wann beginnt der Kurs? → When does the course start?<br>
Warum lernst du Deutsch? → Why are you learning German?<br>
Wie geht es dir? → How are you?<br>
Wieviel kostet das? → How much does it cost?<br>
Welches Buch liest du? → Which book are you reading?
</p>

<h3>2.4 Advanced WH-Questions</h3>

<p><strong>a) Negation:</strong><br>
Warum kommst du nicht? → Why aren’t you coming?<br>
Wieso hast du das nicht gemacht? → Why didn’t you do that?<br>
Wer kann heute nicht kommen? → Who cannot come today?<br>
Was isst du nicht gerne? → What don’t you like to eat?
</p>

<p><strong>b) Modal Verbs:</strong><br>
Wie kann ich dir helfen? → How can I help you?<br>
Was soll ich tun? → What should I do?<br>
Wer darf hier nicht sitzen? → Who is not allowed to sit here?<br>
Wann musst du arbeiten? → When do you have to work?
</p>

<p><strong>c) Separable Verbs:</strong><br>
Wann stehst du auf? → When do you get up?<br>
Was bringst du mit? → What are you bringing along?<br>
Wo fängst du an? → Where do you start?<br>
Wohin gehst du heute? → Where are you going today?
</p>

<p><strong>d) Polite/Formal:</strong><br>
Wie heißen Sie? → What is your name?<br>
Woher kommen Sie? → Where are you from?<br>
Wann haben Sie Zeit? → When do you have time?<br>
Was möchten Sie essen? → What would you like to eat?
</p>

<p><strong>Extra Advanced Examples:</strong><br>
Wer wird das Meeting leiten? → Who will lead the meeting?<br>
Was hast du gestern gemacht? → What did you do yesterday?<br>
Wann habt ihr Urlaub? → When do you have vacation?<br>
Wie lange dauert der Film? → How long does the movie last?<br>
Welche Bücher hast du gelesen? → Which books have you read?<br>
Woher weißt du das? → How do you know that?<br>
Warum hast du das entschieden? → Why did you decide that?
</p>

</body>
</html>
</div>

<!-- Accusative -->
<div id="accusative" class="topic">
    <button class="back-btn" onclick="goBack()">← Back</button>
    <h1>Accusative Case Basics</h1>
    

<h2>1. Definition</h2>
<p>The <strong>Akkusativ</strong> (Accusative case) is used for the <strong>direct object</strong> of a sentence — the person or thing <strong>receiving the action</strong>. It answers the questions: <strong>“Wen?” (Whom?)</strong> and <strong>“Was?” (What?)</strong></p>

<p><strong>Example:</strong> Ich sehe <strong>den Mann</strong>. → I see <strong>the man</strong>.</p>
<p>(Wen sehe ich? → den Mann)</p>

<h2>2. How the Akkusativ is Formed</h2>
<p>In German, the accusative affects:</p>
<ul>
<li>The article of nouns (definite and indefinite)</li>
<li>Personal pronouns</li>
<li>Objects after certain verbs</li>
<li>Objects after certain prepositions</li>
</ul>

<p>Basic structure of a sentence in Akkusativ:</p>
<p><strong>Subject + Verb + Direct Object (Accusative) + Rest</strong></p>

<p><strong>Example:</strong> Ich kaufe <strong>ein Buch</strong>. → I buy <strong>a book</strong>.</p>

<h2>3. Akkusativ Articles</h2>

<h3>3.1 Definite Articles (the)</h3>
<table border="1">
<tr><th>Gender</th><th>Nominative</th><th>Accusative</th></tr>
<tr><td>Masculine</td><td>der</td><td>den</td></tr>
<tr><td>Feminine</td><td>die</td><td>die</td></tr>
<tr><td>Neuter</td><td>das</td><td>das</td></tr>
<tr><td>Plural</td><td>die</td><td>die</td></tr>
</table>

<h3>3.1.1 Examples</h3>
<ul>
<li>Ich sehe <strong>den Hund</strong>. → I see the dog.</li>
<li>Sie kauft <strong>die Blume</strong>. → She buys the flower.</li>
<li>Er liest <strong>das Buch</strong>. → He reads the book.</li>
<li>Wir hören <strong>die Kinder</strong>. → We hear the children.</li>
<li>Ich treffe <strong>den Lehrer</strong>. → I meet the teacher.</li>
</ul>

<h3>3.2 Indefinite Articles (a/an)</h3>
<table border="1">
<tr><th>Gender</th><th>Nominative</th><th>Accusative</th></tr>
<tr><td>Masculine</td><td>ein</td><td>einen</td></tr>
<tr><td>Feminine</td><td>eine</td><td>eine</td></tr>
<tr><td>Neuter</td><td>ein</td><td>ein</td></tr>
<tr><td>Plural</td><td>keine</td><td>keine</td></tr>
</table>

<h3>3.2.1 Examples</h3>
<ul>
<li>Ich sehe <strong>einen Mann</strong>. → I see a man.</li>
<li>Sie kauft <strong>eine Tasche</strong>. → She buys a bag.</li>
<li>Er liest <strong>ein Buch</strong>. → He reads a book.</li>
<li>Wir haben <strong>keine Äpfel</strong>. → We have no apples.</li>
<li>Ich treffe <strong>einen Freund</strong>. → I meet a friend.</li>
</ul>

<h2>4. Akkusativ Pronouns</h2>
<table border="1">
<tr><th>Person</th><th>Nominative</th><th>Accusative</th></tr>
<tr><td>ich</td><td>ich</td><td>mich</td></tr>
<tr><td>du</td><td>du</td><td>dich</td></tr>
<tr><td>er</td><td>er</td><td>ihn</td></tr>
<tr><td>sie</td><td>sie</td><td>sie</td></tr>
<tr><td>es</td><td>es</td><td>es</td></tr>
<tr><td>wir</td><td>wir</td><td>uns</td></tr>
<tr><td>ihr</td><td>ihr</td><td>euch</td></tr>
<tr><td>sie</td><td>sie</td><td>sie</td></tr>
<tr><td>Sie (formal)</td><td>Sie</td><td>Sie</td></tr>
</table>

<h3>4.1 Examples</h3>
<ul>
<li>Sie sieht <strong>mich</strong>. → She sees me.</li>
<li>Ich liebe <strong>dich</strong>. → I love you.</li>
<li>Er kennt <strong>ihn</strong>. → He knows him.</li>
<li>Wir treffen <strong>uns</strong>. → We meet each other.</li>
<li>Sie hört <strong>sie</strong>. → She hears them.</li>
</ul>

<h2>5. Akkusativ Prepositions</h2>
<p>Always take Akkusativ:</p>
<p><strong>durch, für, gegen, ohne, um</strong></p>

<h3>5.1 Examples</h3>
<ul>
<li>Ich gehe <strong>durch den Park</strong>. → I walk through the park.</li>
<li>Das Geschenk ist <strong>für dich</strong>. → The gift is for you.</li>
<li>Er kämpft <strong>gegen den Feind</strong>. → He fights against the enemy.</li>
<li>Sie geht <strong>ohne ihre Tasche</strong>. → She goes without her bag.</li>
<li>Wir sitzen <strong>um den Tisch</strong>. → We sit around the table.</li>
</ul>

<h2>6. Two-Way Prepositions (Wechselpräpositionen)</h2>
<p>Prepositions can take Dativ (location) or Akkusativ (motion/direction).</p>
<p>Common Akkusativ examples (motion/direction):</p>
<ul>
<li>Ich gehe <strong>in die Schule</strong>. → I go into the school.</li>
<li>Er legt das Buch <strong>auf den Tisch</strong>. → He puts the book on the table.</li>
<li>Wir fahren <strong>durch den Wald</strong>. → We drive through the forest.</li>
<li>Sie stellt die Lampe <strong>neben das Sofa</strong>. → She places the lamp next to the sofa.</li>
<li>Er geht <strong>hinter das Haus</strong>. → He goes behind the house.</li>
</ul>

<h2>7. Akkusativ Verbs</h2>
<p>Some verbs always require a direct object (accusative): haben, sehen, kaufen, lieben, kennen, hören</p>

<h3>7.1 Examples</h3>
<ul>
<li>Ich habe <strong>einen Hund</strong>. → I have a dog.</li>
<li>Er sieht <strong>die Frau</strong>. → He sees the woman.</li>
<li>Wir kaufen <strong>das Auto</strong>. → We buy the car.</li>
<li>Sie liebt <strong>ihn</strong>. → She loves him.</li>
<li>Ich kenne <strong>die Stadt</strong>. → I know the city.</li>
</ul>

<h2>8. Akkusativ with Adjective Endings</h2>
<ul>
<li>Ich sehe <strong>den großen Hund</strong>. → I see the big dog.</li>
<li>Sie kauft <strong>eine schöne Tasche</strong>. → She buys a beautiful bag.</li>
<li>Er liest <strong>das interessante Buch</strong>. → He reads the interesting book.</li>
<li>Wir besuchen <strong>die netten Kinder</strong>. → We visit the nice children.</li>
<li>Ich finde <strong>den alten Mann</strong> sympathisch. → I find the old man nice.</li>
</ul>

<h2>9. Negation in Akkusativ</h2>
<ul>
<li>Ich habe <strong>kein Geld</strong>. → I have no money.</li>
<li>Sie sieht <strong>den Hund nicht</strong>. → She does not see the dog.</li>
<li>Wir kaufen <strong>keine Äpfel</strong>. → We buy no apples.</li>
<li>Er liebt <strong>sie nicht</strong>. → He does not love her.</li>
<li>Ich kenne <strong>die Regeln nicht</strong>. → I do not know the rules.</li>
</ul>

<h2>10. Time Expressions (Akkusativ)</h2>
<ul>
<li>Ich gehe <strong>jeden Tag</strong> zur Arbeit. → I go to work every day.</li>
<li>Wir sehen uns <strong>jeden Montag</strong>. → We see each other every Monday.</li>
<li>Er arbeitet <strong>jede Woche</strong> im Büro. → He works in the office every week.</li>
<li>Sie reist <strong>jedes Jahr</strong> nach Deutschland. → She travels to Germany every year.</li>
<li>Ich treffe ihn <strong>jeden Abend</strong>. → I meet him every evening.</li>
</ul>

<h2>Summary</h2>
<p>Akkusativ is used for the <strong>direct object</strong>, after certain verbs, prepositions, and expressions. Articles, pronouns, adjectives, and nouns all change according to gender, number, and case. Using Akkusativ correctly is essential for understanding and forming German sentences.</p>



<h1>German Akkusativ Verbs (Direct Object Verbs)</h1>

<h2>1. Definition</h2>
<p>
Akkusativ verbs are verbs that <strong>require a direct object</strong> to complete their meaning. 
The direct object answers the questions <strong>“Wen?” (Whom?)</strong> or <strong>“Was?” (What?)</strong> 
and takes the <strong>accusative case</strong> in German.
</p>

<h2>2. Usage</h2>
<p>
These verbs always act on something or someone. You can recognize them by asking “Wen/Was?” after the verb. 
For example:
</p>
<ul>
<li>Ich sehe <strong>den Hund</strong>. → I see <strong>the dog</strong>. (Wen sehe ich?)</li>
<li>Sie kauft <strong>ein Buch</strong>. → She buys <strong>a book</strong>. (Was kauft sie?)</li>
<li>Wir hören <strong>die Musik</strong>. → We hear <strong>the music</strong>. (Was hören wir?)</li>
</ul>

<h2>3. List of 50+ Common Akkusativ Verbs</h2>
<table border="1">
<tr>
<th>German Verb</th>
<th>English Meaning</th>
</tr>
<tr><td>sehen</td><td>to see</td></tr>
<tr><td>haben</td><td>to have</td></tr>
<tr><td>kaufen</td><td>to buy</td></tr>
<tr><td>lieben</td><td>to love</td></tr>
<tr><td>kennen</td><td>to know (a person)</td></tr>
<tr><td>hören</td><td>to hear</td></tr>
<tr><td>finden</td><td>to find</td></tr>
<tr><td>brauchen</td><td>to need</td></tr>
<tr><td>zeigen</td><td>to show</td></tr>
<tr><td>lesen</td><td>to read</td></tr>
<tr><td>tragen</td><td>to carry / wear</td></tr>
<tr><td>treffen</td><td>to meet</td></tr>
<tr><td>verkaufen</td><td>to sell</td></tr>
<tr><td>nehmen</td><td>to take</td></tr>
<tr><td>bringen</td><td>to bring</td></tr>
<tr><td>fragen</td><td>to ask</td></tr>
<tr><td>antworten</td><td>to answer (with object)</td></tr>
<tr><td>verstehen</td><td>to understand</td></tr>
<tr><td>kochen</td><td>to cook</td></tr>
<tr><td>schicken</td><td>to send</td></tr>
<tr><td>schlagen</td><td>to hit</td></tr>
<tr><td>schreiben</td><td>to write</td></tr>
<tr><td>studieren</td><td>to study</td></tr>
<tr><td>spielen</td><td>to play</td></tr>
<tr><td>fotografieren</td><td>to photograph</td></tr>
<tr><td>putzen</td><td>to clean</td></tr>
<tr><td>packen</td><td>to pack</td></tr>
<tr><td>prüfen</td><td>to check / examine</td></tr>
<tr><td>probieren</td><td>to try / taste</td></tr>
<tr><td>planen</td><td>to plan</td></tr>
<tr><td>pünktlich machen</td><td>to do on time</td></tr>
<tr><td>reparieren</td><td>to repair</td></tr>
<tr><td>retten</td><td>to save / rescue</td></tr>
<tr><td>riechen</td><td>to smell</td></tr>
<tr><td>rufen</td><td>to call</td></tr>
<tr><td>suchen</td><td>to search / look for</td></tr>
<tr><td>stellen</td><td>to place / put</td></tr>
<tr><td>stoßen</td><td>to push</td></tr>
<tr><td>strecken</td><td>to stretch</td></tr>
<tr><td>streichen</td><td>to paint / spread</td></tr>
<tr><td>wählen</td><td>to choose / elect</td></tr>
<tr><td>warten</td><td>to wait</td></tr>
<tr><td>wecken</td><td>to wake (someone)</td></tr>
<tr><td>wissen</td><td>to know (a fact)</td></tr>
<tr><td>zeichnen</td><td>to draw</td></tr>
<tr><td>zahlen</td><td>to pay</td></tr>
<tr><td>ziehen</td><td>to pull / move</td></tr>
<tr><td>zubereiten</td><td>to prepare (food)</td></tr>
<tr><td>zusehen</td><td>to watch / observe</td></tr>
<tr><td>zweifeln</td><td>to doubt</td></tr>
<tr><td>zwingen</td><td>to force / compel</td></tr>
<tr><td>verlieren</td><td>to lose</td></tr>
</table>

<h2>4. Usage in Sentences</h2>
<ul>
<li>Ich sehe <strong>den Hund</strong>. → I see the dog.</li>
<li>Sie kauft <strong>ein Buch</strong>. → She buys a book.</li>
<li>Wir lieben <strong>die Musik</strong>. → We love the music.</li>
<li>Er kennt <strong>den Lehrer</strong>. → He knows the teacher.</li>
<li>Ich bringe <strong>das Essen</strong>. → I bring the food.</li>
</ul>

</body>
</html>




</body>
</html>
</div>

<script>
    function showCourse(topicId) {
        document.getElementById("home").style.display = "none";
        document.querySelectorAll(".topic").forEach(div => div.style.display = "none");
        document.getElementById(topicId).style.display = "block";
    }

    function goBack() {
        document.querySelectorAll(".topic").forEach(div => div.style.display = "none");
        document.getElementById("home").style.display = "flex";
    }
</script>




</body>
</html>
      
      
      
      
      
      
      
      
      
      
      
    </div>
  </div>

  <script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/12.3.0/firebase-app.js";
    import { getAnalytics } from "https://www.gstatic.com/firebasejs/12.3.0/firebase-analytics.js";
    import { getAuth, signInWithEmailAndPassword, onAuthStateChanged, signOut } from "https://www.gstatic.com/firebasejs/12.3.0/firebase-auth.js";

    const firebaseConfig = {
      apiKey: "AIzaSyAZeeXuf599DrZNU8SnxRSmykrQiZCHx6Q",
      authDomain: "a1html-69aee.firebaseapp.com",
      projectId: "a1html-69aee",
      storageBucket: "a1html-69aee.firebasestorage.app",
      messagingSenderId: "167372112581",
      appId: "1:167372112581:web:38c2a7ed7d9fc576af66ac",
      measurementId: "G-DG74KGNXR5"
    };

    const app = initializeApp(firebaseConfig);
    const analytics = getAnalytics(app);
    const auth = getAuth(app);

    const loginSection = document.getElementById("loginSection");
    const courseSection = document.getElementById("courseSection");
    const loginBtn = document.getElementById("loginBtn");
    const logoutBtn = document.getElementById("logoutBtn");
    const emailInput = document.getElementById("email");
    const passwordInput = document.getElementById("password");
    const errorMsg = document.getElementById("error");

    // Login
    loginBtn.addEventListener("click", async () => {
      const email = emailInput.value;
      const password = passwordInput.value;
      try {
        await signInWithEmailAndPassword(auth, email, password);
        errorMsg.textContent = "";
      } catch (err) {
        errorMsg.textContent = "Login failed: " + err.message;
      }
    });

    // Auth state listener
    onAuthStateChanged(auth, (user) => {
      if (user) {
        loginSection.style.display = "none";
        courseSection.style.display = "block";
      } else {
        loginSection.style.display = "flex";
        courseSection.style.display = "none";
      }
    });

    // Logout
    logoutBtn.addEventListener("click", async () => {
      await signOut(auth);
    });
  </script>

</body>
</html>
