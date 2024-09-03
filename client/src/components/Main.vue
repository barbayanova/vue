<template>
    <main>
        <img src="../assets/img/cabbage.svg" alt="" srcset="" style="margin-right: 20px; grid-area: 1 / 1 / 2 / 2;">
        <p class="text1">Капуста давно и прочно вошла в рацион нашего питания и принадлежит к числу важнейших овощных растений. Она также является неотъемлемой частью таких традиционных блюд, как: борщ, щи, солянка, тушеная капуста, голубцы, капустная запеканка и конечно квашеная капуста.</p>
        <p class="text2">Капуста не только популярный, но и полезный продукт: она богата витаминами А, В1, Р, К, В6, U. Капуста является лидером среди овощей по содержанию витамина С, причем он сохраняется в капусте как при длительном хранении в сыром виде, так и при термической обработке. В ней также много минералов - сера, кальций, калий и фосфор, клетчатки и воды.</p>
        <div class="bottonn" :style="Wbt">
        <img class="div2" :style="btMenu" src="../assets/img/vkontacte.svg">
        <img class="div3" :style="btMenu" src="../assets/img/telegram.svg">
        <img class="div4" :style="btMenu" src="../assets/img/odnoklassniki 1.svg">
        <p class="div1" @click="activeShare">Поделиться</p>
        </div>
    </main>
</template>

<script setup>

import { reactive} from "vue"

const Wbt = reactive({
    hight: '40px'
})
const btMenu = reactive({
    display: 'none'
})

const activeShare = function() {
    btMenu.display = btMenu.display === 'none' ? '' : 'none'
    Wbt.hight = Wbt.hight === '40px' ? '' : '40px'
}

</script>
