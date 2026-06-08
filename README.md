# Produktvision – Security Escape: IT-säkerhet via CLI

*Visionen togs fram under Sprint 0 och är inte helt klar än. Vi ser den som ett levande dokument och kommer förfina den under projektets gång.*

## Vad vi vill bygga och varför

Vi vill göra ett "Escape Room"-spel som körs i terminalen och lär medarbetare grunderna i IT-säkerhet. Vanlig säkerhetsutbildning upplevs ofta som ett tvång, och då blir engagemanget därefter. Vår idé är att göra det till ett spel istället. Spelaren tar sig genom ett antal rum, löser säkerhetsutmaningar längs vägen, och målet är att till slut fly ut och vinna.

## Hur spelet fungerar

Man rör sig rum för rum, och i varje rum finns en utmaning som handlar om IT-säkerhet. Klarar man rummet får man en pusselbit. När man samlat alla pusselbitar kan man låsa upp den sista dörren och vinna.

Man börjar med tre liv. Svarar man rätt får man ett liv till, svarar man fel förlorar man ett. Tar liven slut är spelet över.

Ett av rummen är ett "Hänga gubbe"-moment. Där har man ett visst antal liv och ska gissa rätt ord utifrån ett säkerhetstema. Man får svarsalternativ att välja mellan, och en progress bar visar hur långt man kommit och hur många försök som är kvar.

## Vad spelet ska klara för att bli godkänt

Istället för en lång kravlista håller vi oss till det övergripande:

- Spelet ska gå att köra i terminalen med ett tydligt flöde mellan rummen.
- Livsystemet ska fungera: tre liv från start, +1 vid rätt svar, -1 vid fel, och spelet ska avslutas korrekt när liven tar slut.
- Varje avklarat rum ger en pusselbit, och alla pusselbitar krävs för att låsa upp slutdörren.
- Ett rum ska ha "Hänga gubbe"-logiken med svarsalternativ, liv och progress bar.
- Framsteg ska kunna sparas i JSON.
- Koden ska ligga i lämpliga PS1-/modulfiler och felhanteras med Try/Catch.

## Tanken bakom

Poängen är att spelaren faktiskt ska bli tryggare på riktigt, inte bara klara en utbildning. Därför är rummen byggda så att man först lär sig vad som gäller – till exempel hur man känner igen ett phishing-mejl eller varför starka lösenord spelar roll – och sedan direkt får använda det genom att ta ett beslut i spelet. Då övar man inte bara teorin utan också själva handlingen, alltså att faktiskt göra rätt när det väl gäller. Att rätt svar ger liv och fel svar kostar liv gör att de bra valen fastnar och kan tas med ut i jobbet.

## Ramar

Vi jobbar agilt med korta sprintar och versionshanterar i GitHub. Allt byggs i PowerShell, och vi dokumenterar löpande här i denna README tillsammans med våra reflektioner från daily stand up, sprint review och sprint retrospective.
