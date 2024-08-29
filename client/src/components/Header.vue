<template>
    <header>
        <h1>Полезные свойства капусты</h1>
        <nav :style="asMenu">
            <ul>
                <li @click="activeMenu"><img src="./assets/img/apps 1.svg" alt=""></li>
                <li>Главная</li>
                <li>Блог</li>
                <li>О нас</li>
                <li>Контакты</li>
            </ul>
        </nav>
    </header>
</template>

<script setup>
    import { reactive } from "vue"

    const asMenu = reactive({
        right: '-300px'
    })

    const activeMenu = function() {
        asMenu.right = asMenu.right === '-300px' ? '' : '-300px'
    }
    
</script>