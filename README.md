# LaboReeks Git
## **Labo 4**

In dit vierde labo gaan werken we verder met branches.
We verkennen ook de Pull Requests die je kan maken om branches te mergen via GitHub.

#### **Aanvullende toets op Leho**
Na het afwerken van dit labo heb je op Leho een aanvullende toets met betrekking tot het labo en de leerstof gekoppeld aan het labo.
Je kan/mag de aanvullende toets steeds afleggen gebruik makend van alle bronnen (cursusmateriaal, labo, online bronnen, ...)

### **Labo 4:** *Takenlijst*

- [ ] Open de Git Bash Console op de locatie waar je dit labo wil gaan clonen. Dit kan via een rechtermuisklik op de locatie in kwestie en vervolgens de keuze **Git Bash Here** te selecteren.
>**Tip!** Indien deze optie niet beschikbaar is dan heb je een stap in de aanbevolen installatie in Labo 01 overgeslaan.

- [ ] Zorg ervoor dat de startsituatie *(deze repository)* van het labo op jouw pc **gecloned** wordt. Maak hiervoor gebruik van het passende git commando. 

- [ ]  Ga **na het clonen** via de console naar de gecloonde repository. Dit kan/mag je uiteraard ook doen door de nieuwe aangemaakt folder aan te klikken en hier opnieuw een Git Bash console te openen via de **Git Bash Here** optie.
>**Tip!** Controleer voor je verder werkte of je al dan niet in de juiste git repository zit! Je kan dit snel visueel vaststellen in je console.

### Deel 1: twee parallele feature branches

- [ ] Maak in je lokale repository een nieuwe branch aan. Deze nieuwe branch geef je als naam **dev** mee. Ga vervolgens naar deze nieuwe aangemaakte branch. 
>**Tip!** Denk er aan voor je naar de volgende stap doorgaat om zeker te controleren dat je **niet** langer op de **master** branch aan het werk bent!

- [ ] Zorg met een passend git commando dat je remote repository (GitHub) deze branch, alsook de inhoud ervan, ook binnenkrijgt en tevens linkt aan je lokale branch. 

- [ ] Vanuit je **dev branch** maak je vervolgens **2 nieuwe branches** aan. Deze branches geef je volgende namen:
    -  **feature/portfolio-submarine**
    -  **feature/portfolio-locked-safe**
>**Tip!** Zorg er zeker voor dat je je op de **dev** branch bevindt voor je aan de slag gaat met het aanmaken van nieuwe branches (of gebruik de meer uitgebreide commado's waarbij je expliciet opgeeft dat er vanaf **dev** moet afgetakt worden)

- [ ] Switch een voor een naar deze nieuwe branches en zorg met een passend git commando dat je remote repository *(GitHub)* deze branches, alsook de inhoud ervan, ook binnenkrijgt en tevens linkt aan je lokale branches. 

- [ ] Ga naar de **feature/portfolio-locked-safe** branch en ga vervolgens naar de src folder. Hierin vind je een index.html bestand waar we mee zullen werken. Open het index.html bestand in een editor naar keuze. 
>**Tip!** dubbelklik gerust eerst even op dit html bestand om de huidige inhoud ervan te bekijken in je browser.

- [ ] Pas de index.html file aan door op **regel 103** onderstaande code te plakken.

```
<!-- Portfolio Item 5-->
    <div class="col-md-6 col-lg-4 mb-5 mb-md-0">
        <div class="portfolio-item mx-auto" data-toggle="modal" data-target="#portfolioModal5">
            <div class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100">
                <div class="portfolio-item-caption-content text-center text-white"><i class="fas fa-plus fa-3x"></i></div>
            </div>
                <img class="img-fluid" src="assets/img/portfolio/safe.png" alt="" />
        </div>
    </div>
```

- [ ] Zorg ervoor dat de wijzigingen aan de index.html opgenomen worden in git. Synchroniseer hierna je lokale repository met je online repository.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Ga naar de **feature/portfolio-submarine** branch en open opnieuw het index.html bestand in een editor naar keuze. 
>**Tip!** dubbelklik gerust eerst even op dit html bestand om de huidige inhoud ervan te bekijken in je browser.

- [ ] Pas de index.html file aan door op **regel 103** onderstaande code te plakken.

```
<!-- Portfolio Item 6-->
    <div class="col-md-6 col-lg-4">
        <div class="portfolio-item mx-auto" data-toggle="modal" data-target="#portfolioModal6">
            <div class="portfolio-item-caption d-flex align-items-center justify-content-center h-100 w-100">
                <div class="portfolio-item-caption-content text-center text-white"><i class="fas fa-plus fa-3x"></i></div>
            </div>
            <img class="img-fluid" src="assets/img/portfolio/submarine.png" alt="" />
        </div>
    </div>
```

- [ ] Zorg ook hier dat de wijzigingen aan de index.html opgenomen worden in git. Synchroniseer hierna je lokale repository met je online repository.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

- [ ] Ga naar de **dev** branch en voer onderstaande commandos uit.
```
clear
git remote
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshot folder die je in je labo4 folder staan hebt. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel1** (met extensie naar keuze).

- [ ] Maak gebruik van passende git commando's om alle lokale bestanden te commiten naar git. **Synchroniseer** vervolgens je lokale repository met de online repository op GitHub.
>**Tip!** Denk aan de conventies rondom naamgeving van de commit messages!

### Deel 2: mergen via Pull Request

We gaan nu een voor een de twee feature branches mergen naar **dev** maar **NIET** lokaal.
Hiervoor gebruiken we de **Pull Requests** op GitHub.

- [ ] Maak in je remote repo op GitHub een eerste Pull Request aan die de branch **feature/portfolio-locked-safe** wenst te mergen in **dev**.
 
- [ ] Verifieer dat er zich geen conflicten voordoen en accepteer de Pull Request, zodat **feature/portfolie-locked-safe** effectief in **dev** wordt gemerged op je remote repo.

- [ ] Lokaal bevind je je normaal gezien nog steeds op de **dev** branch. Zo niet: ga dan terug naar de **dev** branch.
- [ ] Zorg ervoor dat je lokale **dev** branch de wijzigingen vanuit de remote binnenkrijgt.

- [ ] Maak een screenshot van je Pull Request pagina op GitHub, waarop duidelijk te zien is dat de PR werd gemerged en bijgevolg afgesloten is. Deze screenshot plaats je in de **lokale** Screenshot folder die je in je labo4 folder staan hebt. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel2** (met extensie naar keuze).

- [ ] Gebruik de gepaste git commando's om de toegevoegde screenshot lokaal op te nemen in git (op de **dev** branch) en ook naar de remote te syncen.

### Deel 3: Pull Request met merge conflict

- [ ] Maak een tweede Pull Request, deze keer van de branch **feature/portfolio-submarine** naar **dev**. Hier zal er een conflict ontstaan waardoor de Pull Request niet onmiddelijk aanvaard kan worden.

- [ ] Maak een screenshot van (het deel van) je Pull Request waarop duidelijk te zien is dat er een conflict is en dat de PR bijgevolg niet zomaar kan gemerged worden. Deze screenshot plaats je in de **lokale** Screenshot folder die je in je labo4 folder staan hebt. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel3** (met extensie naar keuze).

- [ ] Gebruik de gepaste git commando's om de toegevoegde screenshot lokaal op te nemen in git (op de **dev** branch) en ook naar de remote te syncen.

### Deel 4: merge conflict oplossen (lokaal)

We gaan nu het conflict dat zich voordoet in de tweede Pull Request oplossen zodat **zowel de locked safe als de submarine** in de index.html blijven staan. We willen dus de wijzigingen van beide feature branches behouden en die gewoon onder elkaar plaatsen in de finale merge. We gaan dit conflict **lokaal** oplossen (**NIET** rechtstreeks op GitHub).

- [ ] Ga in je Git Bash console (dus lokaal) naar de branch **feature/portfolio-submarine**.
- [ ] Merge **dev** in **feature/portfolio-submarine** en maak een screenshot van het gebruikte git commando en de output ervan. Deze screenshot plaats je in de **lokale** Screenshot folder die je in je labo4 folder staan hebt. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel4** (met extensie naar keuze).
>**Tip!** Aangezien we middenin een merge met conflictoplossing zitten, laten we de net toegevoegde screenshot gewoon even staan in de working directory zonder ze al op te nemen in de git geschiedenis. Straks bij het afronden van de merge nemen we deze gewoon mee met de andere aanpassingen.

- [ ] Los het conflict nu lokaal op door **zowel de locked safe als de submarine** in de index.html te laten staan (onder elkaar).
- [ ] Gebruik de gepaste git commando's om de merge af te ronden, waarbij de oplossing van het conflict in de lokale geschiedenis belandt. **Let op:** zorg er hier voor dat ook de zonet toegevoegde vierde screenshot mee opgenomen wordt in de merge commit.

- [ ] Synchroniseer de lokale wijzigingen aan de branch **feature/portfolio-submarine** nu ook naar de remote repo.
- [ ] Accepteer tenslotte de tweede Pull Request op GitHub zodat **feature/portfolio-submarine** effectief in **dev** wordt gemerged.

### Deel 5: afronden labo

- [ ] Ga lokaal naar de **dev** branch en zorg ervoor dat je de laatste wijzigingen vanuit de remote hier binnentrekt.
- [ ] Na het voltooien van alle taken editeer je deze README.md file.
      **LET OP!** dit doe je opnieuw in je lokale README.md file!
      Plaats alle tasks op voltooid door de markup te wijzigen van [ ] naar [x].
>**Tip!** Je kan hier gerust VS Code gaan gebruiken. Deze heeft ook een preview mode om met markdown aan de slag te gaan.

- [ ] Maak gebruik van git commando's om vervolgens deze wijzigingen aan je lokale git repository toe te voegen.
      Sync de lokale **dev** branch vervolgens naar de remote.

- [ ] Voer hierna onderstaande commandos uit.
```
clear
git branch
git log --oneline
```

- [ ] Neem een screenshot van het resultaat. Deze screenshot plaats je in de **lokale** Screenshot folder die je in je labo4 folder staan hebt. *(Op jouw PC/laptop dus!)* Geef deze screenshot de naam **deel5** (met extensie naar keuze).
- [ ] Gebruik de gepaste git commando's om de toegevoegde screenshot lokaal op te nemen in git (op de **dev** branch) en ook naar de remote te syncen.

- [ ] Maak nog een laatste Pull Request op je remote repo die **dev** in **master** wenst te mergen.
- [ ] Verifieer dat er geen conflicten ontstaan en accepteer de Pull Request.
