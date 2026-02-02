<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Dutch Airstrikes',
        description: `Im Airwars-Archiv befinden sich 2.978 mutmaßliche Fälle, in denen Zivilisten durch die US-geführte Koalition im Krieg gegen den IS zu Schaden kamen. Die Zahl der Getöteten wird auf mindestens 8.000 geschätzt. Zwar räumte die Koalition über 300 dieser Vorfälle ein, doch bislang erkannten nur vier Mitgliedstaaten – darunter die Niederlande – Schäden durch ihre eigene Beteiligung an. Im Rahmen des Projekts wurden Standorte aus dem Airwars-Archiv mit Daten des niederländischen Verteidigungsministeriums abgeglichen. Nach einjähriger Zusammenarbeit legte das Ministerium dem Parlament detaillierte Ergebnisse zu 61 von Airwars identifizierten Vorwürfen ziviler Schäden im Umfeld niederländischer Luftangriffe im Irak und in Syrien vor.`,
        year: '2025',
        link: 'https://airwars.org/dutch-mod-releases-results-of-largest-ever-assessment-of-civilian-harm-allegations-from-the-war-against-isis/',
        linkName: 'Airwars Report',
        collaborators: 'Megan Karlshoej-Pedersen<br>& Clive Vella'
    };
    export let items = [
        { image: 'assets/proj6-img1.jpg', title: 'Overview of strikes in Iraq and Syria', id: 1, isHovered: false },
        { image: 'assets/proj6-img2.jpg', title: 'Analyse von niederländischen Angriffen und Airwars-Archivdaten für Hajin', id: 2, isHovered: false },
        { image: 'assets/proj6-img3.jpg', title: 'Analyse von niederländischen Angriffen und Airwars-Archivdaten für Aski Mosul', id: 3, isHovered: false }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>