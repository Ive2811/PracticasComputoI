<template>
    <div id="app">
        <nav class="navbar navbar-light bg-light">
            <div class="container-fluid">
                <span class="navbar-brand">
                    {{title}}
                </span>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name:'HeaderTitle',
    props:{
        title: String
    }    
}
</script>