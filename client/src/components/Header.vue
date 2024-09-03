<template>
    <header>
        <h1 v-if="asHead">Полезные свойства капусты</h1>
        <nav :style="asMenu">
            <button @click="activeMenu"><img src="../assets/img/apps 1.svg" alt=""></button>
            <ul>
                <li>Главная</li>
                <li>Блог</li>
                <li>О нас</li>
                <li>Контакты</li>
            </ul>
        </nav>
    </header>
</template>

<script setup>
    import { reactive, ref } from "vue"
    const asHead = ref(true)

    const asMenu = reactive({
        right: '-300px',
        width:'370px',
    })

    const activeMenu = function() {
        asMenu.right = asMenu.right === '-300px' ? '' : '-300px'
        asMenu.width = asMenu.width === '370px' ? '' : '370px'
        asHead.value = !asHead.value
    }
    
</script>
<style>
</style>