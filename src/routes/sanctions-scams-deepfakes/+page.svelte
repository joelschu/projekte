<script>
    import ProjectInfo from '$lib/components/ProjectInfo.svelte';

    import  ProjectImageScroll from '$lib/components/ProjectImageScroll.svelte';

    export let projectInfo = {
        title: `Mapping Shark Island`,
        description: 'lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
        year: '2024',
        link: 'https://forensic-architecture.org/investigation/shark-island',
        linkName: 'Forensic Architecture'
    };
    export let items = [
        // { image: 'assets/proj5-img-cover.jpg', title: 'Map Eurasia', id: 1, isHovered: false },
        // // { image: 'assets/proj5-img2.jpg', title: 'Map Eurasia', id: 1, isHovered: false },
        // { image: 'assets/proj5-img3.jpg', title: 'Map Eurasia', id: 1, isHovered: false },
        // { image: 'assets/proj5-img4.jpg', title: 'Map Eurasia', id: 1, isHovered: false }
    ]
</script>

<ProjectInfo {projectInfo}/>

<ProjectImageScroll {items}/>