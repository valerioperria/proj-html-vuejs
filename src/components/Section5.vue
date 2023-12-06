<script>
export default {
    data() {
        return {
            cards: [
                {
                    title: "Increasing creativity is possible for everyone",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                    user: "Andrea Miller",
                    access: "2 Days Ago",
                    class: "class1"
                },
                {
                    title: "Because market research is part of the business plan",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                    user: "Kevin Heart",
                    access: "1 Hour Ago",
                    class: "class2"
                },
                {
                    title: "Working from home is now a trend",
                    text: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
                    user: "Monica Johnson",
                    access: "1 Days Ago",
                    class: "class3"
                },
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <h5><strong>OUR EDITORIAL CONTENT</strong></h5>
            <h1><strong>Latest</strong><strong class="news">News</strong></h1>
            <div class="pEButton">
                <p>Every week we publish content about what is best in the business world.</p>
                <button>SEE ALL</button>
            </div>
        </div>
        <div class="cards">
            <div class="card" v-for="card in cards" :class="card.class">
                <div class="userEaccess">
                    <div class="user"><i class="fa-solid fa-user"></i><span>{{ card.user }}</span></div>
                    <div class="access"><i class="fa-solid fa-clock"></i><span>{{ card.access }}</span></div>
                </div>
                <h3>{{ card.title }}</h3>
                <p>{{ card.text }}</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    padding: 120px 350px;
    .wrapper {
        margin-bottom: 3rem;

        h5 {
            color: $nex;
            margin-bottom: 2rem;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;

            .news {
                background-color: $primaryBg;
                color: $primaryColor;
                padding: 0.5rem;
                margin-left: 0.5rem;
                border-radius: 6px;
            }
        }

        .pEButton {
            @include flex(flex, row, space-between, center, nowrap, 0);

            button {
                @include button;
                width: 8rem;
                margin-left: 200px;
            }
        }
    }

    .cards {
        width: 100%;
        @include flex(flex, row, space-between, center, wrap, 2rem);

        .card {
            width: calc((100% / 3) - 2rem);
            height: 350px;
            border-radius: 12px;
            @include flex(flex, column, end, center, nowrap, 0);
            padding: 2rem 1rem;

            .userEaccess {
                @include flex(flex, row, base-line, center, wrap, 2rem);
                display: none;

                i {
                    margin-right: 4px;
                }
            }

            h3 {
                text-align: center;

            }

            p {
                text-align: center;
                display: none;
            }

            &:hover {
                justify-content: space-between;

                .userEaccess {
                    display: flex;
                }

                p {
                    display: block;
                }
            }
        }

        .class1 {
            background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url(../assets/img/news-1.jpg);
            background-size: cover;
            color: white;

            &:hover {
                background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url(../assets/img/news-1.jpg);
                background-size: cover;
            }
        }

        .class2 {
            background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url(../assets/img/news-2.jpg);
            background-size: cover;
            color: white;

            &:hover {
                background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url(../assets/img/news-2.jpg);
                background-size: cover;
            }
        }

        .class3 {
            background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url(../assets/img/news-3.jpg);
            background-size: cover;
            color: white;

            &:hover {
                background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url(../assets/img/news-3.jpg);
                background-size: cover;
            }
        }

    }
}</style>
