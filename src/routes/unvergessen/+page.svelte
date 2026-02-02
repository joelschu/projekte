<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Un<br>vergessen',
        description: 'Ausgehend von einem Haufen Grabsteinresten im hinteren Bereich eines bekannten Friedhofs in Weimar, Deutschland, untersucht dieses Projekt die Rolle und Politik des Alterns und des Vergessens. Mithilfe der Photogrammetrie wird die Physikalität der Erinnerung in einen digitalen Raum übertragen und hinterfragt nicht nur, wer in Erinnerung bleibt, sondern auch, wie man in einem Zeitalter der digitalen Überwachung und permanenten Aufzeichnungen in Vergessenheit geraten kann. Auf vielen verschiedenen Grabsteinen eingraviert, wird „Unvergessen” weniger zu einer leeren Phrase als vielmehr zu einer Frage.',
        year: '2022',
        link: 'https://www.m-books.eu/store/horizonte-16/',
        linkName: 'Publiziert in Horizonte 16',
        collaborators: 'Charlotte Flügger'
    };
    export let items = [
        { image: 'src/lib/assets/proj7-vid1.mov', title: 'video-grabstein', id: 1, isHovered: false },
        { image: 'src/lib/assets/proj7-vid1.mov', title: 'video-grabstein', id: 2, isHovered: false }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>