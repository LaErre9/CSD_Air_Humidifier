<img src="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/LogoAirHumidifier.png?raw=true" alt="Alt text" title="Logo Air " width="auto" height="auto">
"L’elettricità statica nei nostri capelli o le scintille che volano quando si tocca qualcuno o qualcosa (e.g maniglia) in inverno e non solo sono sicuramente segnali che l’aria nella nostra casa è troppo secca."

Soluzione? **UMIDIFICATORE**

L’inverno è il periodo migliore per utilizzare un umidificatore poiché la temperatura sarà bassa e il livello di umidità relativa scenderà al di sotto del 30%-40%. 
Durante la fredda stagione, nelle nostre case accendiamo il riscaldamento. Senza la possibilità di aprire le finestre, l’aria calda non ricircolata asciugherà l’umidità nella stanza lasciando l’aria viziata, secca e scomoda da respirare.

Cosa può compromettere? Alcuni sintomi:

- Naso che cola cronico
- Sintomi di febbre 
- Asma e riacutizzazioni di allergie
- Gola secca

Occhio anche ai mobili di legno della nostra casa, che possono danneggiarsi deformandosi.

## L'obiettivo
L’obiettivo è realizzare un umidificatore in grado di attivarsi in maniera automatica e portare dopo un certo tempo di transizione l’umidità nell’ambiente intorno alle percentuali indicate nel seguente **infographic della National Asthma Council Australia**.
<center><img src="https://i1.wp.com/www.sensitivechoice.com/wp-content/uploads/2015/04/20140624_Graph-1024x640.jpg?resize=1024%2C640&ssl=1" alt="Alt text" title="Logo Air " width="600" height="auto"></center>

## Componentistica
- 2xDiscovery Kit STM32F3 DISCOVERY
- Sensore livello dell'acqua
- Sensore Temperatura e umidità
- OLED Display
- Nebulizzatore with Grove
- Jumpers

## Architettura Concettuale
<center><img src="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/ArchitetturaConcettuale.png?raw=true" alt="Alt text" title="Logo Air " width="800" height="auto"></center>

- **NODO A**: *Trasmette* al nodo B l'accensione del nebulizzatore se non rispetta i vincoli Temp/Umidità -> *Riceve* dal nodo B il livello dell’acqua basso e mostrarlo a video
- **NODO B**: *Trasmette* al nodo A livello dell’acqua insufficiente -> *Riceve* dal nodo A il segnale di abilitazione del nebulizzatore

## Architettura Complessiva
<center><img src="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/ArchitetturaComplessiva.png" alt="Alt text" title="Logo Air " width="auto" height="auto"></center>

## Protocolli, automi e altro
Segui il pdf! <a href="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/AirHumidifier_Doc_Slide.pdf">Documentazione</a>



# Interconnessioni Nodo A - Nodo B
<center><img src="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/InterconnessioneNodi.png?raw=true" alt="Alt text" title="Logo Air " width="auto" height="auto"></center>

## Immagini
*Overview Nodo A - Nodo B*
<center><img src="https://raw.githubusercontent.com/LaErre9/CSD_Air_Humidifier/main/Filmati/Overview.png" alt="Alt text" title="Logo Air " width="500" height="auto"></center>

*Overview Nodo B*
<center><img src="https://raw.githubusercontent.com/LaErre9/CSD_Air_Humidifier/main/Filmati/Overview2.png" alt="Alt text" title="Logo Air " width="500" height="auto"></center>

# Video illustrativi
Simulazione funzionamento : <a href="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/Simulazione_funzionamento_nebulizzatore.mov">Nebulizzatore</a><br>
Simulazione mancanza: <a href="https://github.com/LaErre9/CSD_Air_Humidifier/blob/main/Filmati/Simulazione_mancanza_acqua.mov">Acqua</a>

# Progetto realizzato per soli scopi dimostrativi e didattici
Nella seguente trattazione è mostrato un progetto STM32 per sistemi embedded richiesto per l'esame di Computer System Design all'Università degli Studi di Napoli Federico II, A.A 2021-2022.

***Autori***<br>
Antonio Romano<br>
Giuseppe Riccio<br>















