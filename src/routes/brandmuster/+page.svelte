<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Brandmuster',
        description: `‚Brandmuster‘ untersucht das wiederkehrende Phänomen von Bränden in Geflüchtetenunterkünften und Wohnräumen von Migranten. Die Untersuchung von Brandereignissen – sei es durch Brandstiftung durch rechtsextreme Täter*innen, durch Bewohner*innen oder durch technische Defekte – ermöglicht es, die komplexen Zusammenhänge der deutschen Migrationspolitik und der damit verbundenen Praktiken zu beleuchten, die Asylsuchende immobilisieren und sie gleichzeitig dem Risiko von vorsätzlichen und unbeabsichtigten Bränden aussetzen. Die Daten wurden auf einer Archiv-Website zusammengestellt, die eine scrollbare Zeitleiste mit Brandereignissen enthält.`,
        year: '2024',
        link: 'https://brandmuster.info',
        linkName: 'brandmuster.info'
    };
    export let items = [
        { image: 'assets/proj1-img1.jpg', title: 'Image 1' },
        { image: 'assets/proj1-img2.jpg', title: 'Image 2' },
        { image: 'assets/proj1-img-cover.jpg', title: 'Image 3' },
        { image: 'assets/proj1-img-cover.jpg', title: 'Image 4' },
        { image: 'assets/proj1-img-cover.jpg', title: 'Image 5' },
        { image: 'assets/proj1-img-cover.jpg', title: 'Image 6' }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>