<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <h5><strong>NEWSLETTER</strong></h5>
            <h1><strong class="know">Know</strong><strong>First</strong></h1>
            <p>Follow closely and receive content about our company and the current market.</p>
        </div>
        <div class="subscribe">
            <input type="text" value="Name">
            <input type="mail" value="Email">
            <button>SUBSCRIBE</button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    padding: 160px 400px;
    @include flex(flex, row, base-line, center, nowrap, 0);
    background-image: url(../assets/img/bg-1.jpg);
    background-size: cover;
    background-position: center;

    .wrapper {
        width: 50%;

        h5 {
            color: $nex;
            margin-bottom: 2rem;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;
            color: white;

            .know {
                background-color: $primaryBg;
                padding: 0.5rem;
                margin-right: 0.5rem;
                border-radius: 6px;
            }
        }

        p {
            color: white;
        }
    }

    .subscribe {
        width: 50%;

        @include flex(flex, column, base-line, baseline, nowrap, 0);

        input {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            background-color: rgba(255, 255, 255, 0.575);
            border: none;
            border-radius: 6px
        }

        button {
            @include button;
        }
    }
}
</style>
