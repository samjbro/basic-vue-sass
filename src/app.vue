<template>
    <div id="app">
        <main-header />
        <main-content />
    </div>
</template>

<script>
    import MainHeader from '@/components/layouts/main-header';
    import MainContent from '@/components/layouts/main-content';
    export default {
        name: 'App',
        components: {MainHeader, MainContent}
    }
</script>