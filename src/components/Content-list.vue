<script setup lang="ts">
    let contentList = [
        {
            "details": 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        },
        {
            "details": 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        },
        {
            "details": 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
        }
    ]
</script>

<template>
  <div class="">
    <div class="content-list__container">
        <ul class="content-list">
            <li class="content-list__item" v-for="contentItem in contentList">
                <div class="content-list__img"></div>
                <p>{{ contentItem.details }}</p>
                <a href="#">Read more</a>
            </li>
        </ul>
    </div>
  </div>
  
</template>

<style scoped>
.content-list__img {
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-image: url(../assets/content-banner.png);
    border-radius: 5px;
    width: 100%;
    min-height: 300px;
}

.content-list {
    margin: 50px 20px;
}
.content-list__item {
    border: 2px solid #ededed;
    border-radius: 10px;
    padding: 15px;
    text-align: center;
    margin-top: 20px;
}
.content-list__item p {
    margin: 10px 0;
}
.content-list__item a {
    border: 3px solid #333333;
    color: #333333;
    font-weight: 700;
    border-radius: 20px;
    height: 40px;
    display: inline-block;
    line-height: 34px;
    text-decoration: none;
    text-transform: uppercase;
    letter-spacing: 0.10em;
    padding: 0 15px;
}
@media (min-width: 1024px) {
    .content-list {
        display: flex;
        gap: 20px;
        justify-content: center;
    }
    .content-list__item {
        max-width: 375px;
    }
}
</style>
