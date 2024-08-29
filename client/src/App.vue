<template>
        <Header />
        <main>
            <img src="./assets/img/cabbage.svg" alt="" srcset="" style="margin-right: 20px;">
            <p class="text" style="height: 259px; width: 461px; margin: 51px 43px 0 0;">Капуста давно и прочно вошла в рацион нашего питания и принадлежит к числу важнейших овощных растений. Она также является неотъемлемой частью таких традиционных блюд, как: борщ, щи, солянка, тушеная капуста, голубцы, капустная запеканка и конечно квашеная капуста.</p>
            <p class="text" style="height: 160px; width: 907px; margin: 51px 43px 0 0;">Капуста не только популярный, но и полезный продукт: она богата витаминами А, В1, Р, К, В6, U. Капуста является лидером среди овощей по содержанию витамина С, причем он сохраняется в капусте как при длительном хранении в сыром виде, так и при термической обработке. В ней также много минералов - сера, кальций, калий и фосфор, клетчатки и воды.</p>
            <div class="bottom">
                <img class="div2" src="./assets/img/vkontacte.svg">
                <img class="div3" src="./assets/img/telegram.svg">
                <img class="div4" src="./assets/img/odnoklassniki 1.svg">
                <p class="div1">Поделиться</p>
            </div>
        </main>
        <footer></footer>
</template>

<script setup>
import Header from "./components/Header.vue"




</script>

<style>
header {
    background-color: #FECFB0;
    display: flex;
    position: relative;
    height: 100px;
    text-align: center;
    align-items: center;
    justify-content: center;
    color: #B54B62;
}
nav {
    background-color: #B54B62;
    border-radius: 40px;
    padding: 10px 30px;
    position: absolute;
    top: 30px;
    right: -290px;
    transition: all 1s linear;
}
ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 25px;
    color: #E5847B;
    font-size: 15px;
    height: 20px;
}
.text {
    color: #B54B62;
    font-size: 24px;
    text-align: justify;

}
li:hover {
    color: #FECFB0;
}
main {
    background-color: #FEA896;
    border-radius: 60px 60px 0px 0px;
    display:  flex;
    flex-wrap: wrap;
    padding: 20px;
}
.bottom {
    height: 80px;
    width: 180px;
    background-color: #B54B62;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    align-items: center;
    text-align: center;
    justify-items: center;
    border-radius: 10px 10px 0px 0px;
    }
        
        .div1 { grid-area: 2 / 1 / 3 / 4; }
        .div2 { grid-area: 1 / 1 / 2 / 2; }
        .div3 { grid-area: 1 / 2 / 2 / 3; }
        .div4 { grid-area: 1 / 3 / 2 / 4; }
p {
    color: #E5847B;
}
</style>