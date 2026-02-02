<script>
    export let projectInfo;
</script>

<div class="header-bar-project">
    <div class="header-bar-project-content">
        <p class="title">
            {@html projectInfo.title}
        </p>
        <p class="legend-header">
                Info
            </p>
        <p class="description-header">
                Über das Projekt
            </p>
            <p class="back-symbol"><a href="/">
        Zurück &#10005;
            </a>
        </p>
    </div>

    <div class="legend">
        
        <div class="legend-block">
            <p class="legend-title">
            von
            </p>
            <p class="legend-text">
                {projectInfo.year}
            </p>
        </div>
        <div class="legend-block">
            <p class="legend-title">
                link
            </p>
            <p class="legend-text">
                <a href={projectInfo.link} target="_blank">{projectInfo.linkName}</a>
            </p>
        </div>
        <div class="legend-block">
            <p class="legend-title">
                mit
            </p>
            <p class="legend-text">
                {@html projectInfo.collaborators}
            </p>
        </div> 
    </div>

<div class="description-container">
    
    <p class="description">
    {projectInfo.description}
</p>
</div>  
</div>
    

