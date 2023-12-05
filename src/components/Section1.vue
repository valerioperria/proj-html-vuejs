<script>
export default {
    data() {
        return {
            cards: [
                {
                    icon: "fa-solid fa-user-group",
                    title: "Human Capital",
                    text: "Humanizing business: harness the power of technology to improve the way people work.",
                },
                {
                    icon: "fa-solid fa-chart-pie",
                    title: "Core Business",
                    text: "It takes innovative approaches to transform, modernize, and runn existing platforms.",
                },
                {
                    icon: "fa-solid fa-gauge-high",
                    title: "Performance",
                    text: "Achieving maximun impact and value from investments in finance and supply chain.",
                },
            ],

        };
    },
}
</script>

<template>
    <div class="container">
        <div class="card" v-for="item in cards">
            <i :class="item.icon"></i>
            <h2>{{ item.title }}</h2>
            <p>{{ item.text }}</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container{
    @include  flex(flex, row, center, center, wrap, 2.5rem);
    background-color: $bgSectionLight;
    width: 100%;
    height: 550px;
    padding: 0 350px;
    .card{
        width: 370px;
        height: 300px;
        @include  flex(flex, column, center, baseline, wrap, 1rem);
        padding: 2rem;
        border-radius: 12px;
        background-color: white;
        &:hover{
            margin-bottom: 1.5rem;
        }
        i{
            color: $primaryColor;
            font-size: 1.5rem;
            background-color: $primaryBg;
            width: 60px;
            height: 60px;
            line-height: 60px;
            border-radius: 50%;
            text-align: center;
        }
    }
}
</style>
