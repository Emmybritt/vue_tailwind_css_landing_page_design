<template>
    <div>
        <div class="sticky z-50 shadow-sm bg-white top-0">
            <HeaderComponent />
        </div>
        <router-view></router-view>
        <FooterComponent />
    </div>
</template>

<script setup>
    import HeaderComponent from '../components/HeaderComponent.vue'
    import FooterComponent from '../components/FooterComponent.vue'
</script>