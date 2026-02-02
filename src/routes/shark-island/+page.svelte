<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Mapping Shark Island',
        description: 'Zwischen 1904 und 1908 findet der erste deutsche Genozid des 20. Jahrhunderts in Namibia statt. Auf der Peninsula Shark Island, eines von fünf Konzentrationslagern der Deutschen ‚Schutztruppen‘, bei Lüderitz sterben zwischen 1905 und 1907 4000 Herero und Nama. Heute ist Shark Island eine touristische Destination, die grausame Geschichte ist überprägt von einem Campingplatz. Über 3D-Scans der Felsstrukturen, Archivbilder und Kartierungsdaten versucht dieses Projekt die Spuren der deutschen Kolonialzeit zu rekonstruieren und dem status quo gegenüberzustellen.',
        year: '2024',
        link: 'https://forensic-architecture.org/investigation/shark-island',
        linkName: 'Forensic Architecture',
        collaborators: 'Agata Nguyen Chuong<br>& Ashkan Cheheltan'
    };
    export let items = [
        { image: 'assets/proj3-img-cover.jpg', title: 'Karte von Shark Island mit Konzentrationslagerstrukturen in rot', titleEng: 'Map of Shark Island with concentration camp structures in red', id: 1, isHovered: false }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>