<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: 'Der Montag',
        description: `Die Zeitung ‚Der Montag‘ setzt sich mit dem Phänomen der Montagsspaziergänge in Weimar auseinander. Abstammend von den Querdenken-Demonstrationen schallt jeden Montag eine Kakophonie von Stimmen durch die Straßen der Kleinstadt: es geht um die Aufklärung der Corona- Verbrechen, um die freie Zukunft der Kinder, den Frieden in Deutschland, den Kampf gegen Insekten im Essen, um die Rettung des Sozialsystems... Der Montag bildet eine kritische Gegenstimme zu den Montagsspaziergängen und eine Sammlung von Kommentaren aus der Stadtgesellschaft Weimars, die den rechten, demokratiefeindlichen und verschwörungsidelogischen Tendenzen in der Bewegung widersprechen.`,
        year: '2023',
        link: 'assets/der_montag_final-version.pdf',
        linkName: 'Der Montag',
        collaborators: 'Pauline Boenisch<br>& Paula Holzhauer'
    };
    export let items = [
        { id: 1, image: 'assets/proj2-img1.jpg', title: 'Cover', isHovered: false },
        { id: 2, image: 'assets/proj2-img-cover.jpg', title: 'Seite 8', isHovered: false },
        { id: 3, image: 'assets/proj2-img3.jpg', title: 'Seite 8', isHovered: false },
        { id: 4, image: 'assets/proj2-img4.jpg', title: 'Seite 6 & 7', isHovered: false },
        { id: 5, image: 'assets/proj2-img5.jpg', title: 'Seite 7', isHovered: false },
        { id: 6, image: 'assets/proj2-img6.jpg', title: 'Seite 2 & 3', isHovered: false }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>