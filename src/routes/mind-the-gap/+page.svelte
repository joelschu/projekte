<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Mind The Gap',
        description: 
        'Im letzten Jahrzehnt sind Zehntausende Menschen auf ihrer Reise nach Europa ertrunken. Das Mittelmeer ist zu einem Ort politischer Machtproben geworden. Trotz der unermüdlichen Arbeit von Menschenrechtsorganisationen und Individuen haben sich staatliche Verbrechen und Menschenrechtsverletzungen naturalisiert. Die Absicht dieses Entwurfs ist es, die Flüchtlingskatastrophe in einem Objekt zu verkörpern, das einerseits als Ort der Sicherheit und andererseits als Mahnmal verstanden werden kann.',
        year: '2020',
        link: 'https://www.koozarch.com/interviews/mind-the-gap',
        linkName: 'KoozArch Interview',
        collaborators: 'Charlotte Flügger',
    };
    export let items = [
        { image: 'src/lib/assets/proj4-img1.jpg', title: 'Status Quo vs Intervention', id: 1, isHovered: false },
        { image: 'src/lib/assets/proj4-img2.jpg', title: 'Konzept der Boje', id: 2, isHovered: false },
        { image: 'src/lib/assets/proj4-img-cover.jpg', title: 'Mittlmeer und die europäische Küste', id: 3, isHovered: false },
        { image: 'src/lib/assets/proj4-img4.jpg', title: 'Die Boje', id: 4, isHovered: false }
    ]

</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>