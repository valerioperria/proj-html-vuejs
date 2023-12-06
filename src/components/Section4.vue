<script>
export default {
    data() {
        return {
            cards: [
                {
                    icon: "fa-solid fa-rocket",
                    title: "Standard",
                    price: "490",
                    class: "standard",
                    list: [
                        {
                            name: "Standard Accounting",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Platform Access",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Business Orientation",
                            tick: "fa-solid fa-x",
                        },
                        {
                            name: "Dedicated Consultant",
                            tick: "fa-solid fa-x",
                        },
                        {
                            name: "Personal Assistance",
                            tick: "fa-solid fa-x",
                        },
                    ]
                },
                {
                    icon: "fa-solid fa-suitcase",
                    title: "Professional",
                    price: "890",
                    ticket: "Most Popular",
                    class: "popular",
                    list: [
                        {
                            name: "Standard Accounting",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Platform Access",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Business Orientation",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Dedicated Consultant",
                            tick: "fa-solid fa-x",
                        },
                        {
                            name: "Personal Assistance",
                            tick: "fa-solid fa-x",
                        },
                    ]
                },
                {
                    icon: "fa-solid fa-gem",
                    title: "Ultimate",
                    price: "1.390",
                    class: "ultimate",
                    list: [
                        {
                            name: "Standard Accounting",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Platform Access",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Business Orientation",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Dedicated Consultant",
                            tick: "fa-solid fa-check",
                        },
                        {
                            name: "Personal Assistance",
                            tick: "fa-solid fa-check",
                        },
                    ]
                },
            ],

        };
    },
}
</script>

<template>
    <div class="container">
        <h5><strong>MONTHLY PLANS</strong></h5>
        <h1><strong class="pricing">Pricing</strong><strong>Table</strong></h1>
        <p>We can help you deliver and execute your future, wherever you compete, using the latest technologies, from
            strategy development to implementation.</p>
        <div class="cards">
            <div class="card" v-for="card in cards" :class="card.class">
                <i class="fa-solid fa-arrow-right arrow"></i>
                <span class="ticket">{{ card.ticket }}</span>
                <i :class="card.icon"></i>
                <h2>{{ card.title }}</h2>
                <h3>$ <span>{{ card.price }}</span> / mo</h3>
                <ul>
                    <li v-for="item in card.list"><span>{{ item.name }}</span><i :class="item.tick"></i></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    height: 920px;
    @include flex(flex, column, baseline, center, nowrap, 0);
    padding: 100px 350px;
    background-color: $bgSectionLight;

    h5 {
        color: $nex;
        margin-bottom: 2rem;
    }

    h1 {
        font-size: 3rem;
        margin-bottom: 2rem;

        .pricing {
            background-color: $primaryBg;
            color: $primaryColor;
            padding: 0.5rem;
            margin-right: 0.5rem;
            border-radius: 6px;
        }
    }

    p {
        text-align: center;
        max-width: 60%;
        margin-bottom: 3rem;
    }

    .cards {
        @include flex(flex, row, space-between, center, wrap, 2rem);
        width: 100%;
        height: 460px;

        .card {
            @include flex(flex, column, baseline, center, wrap, 1rem);
            background-color: white;
            width: calc((100% / 3) - 2rem);
            padding: 1.5rem;
            position: relative;
            border-radius: 12px;

            i {
                font-size: 2.5rem;
                color: $primaryColor;
            }

            h3 {
                color: $primaryColor;
                margin-bottom: 1rem;

                span {
                    font-size: 2rem;
                }
            }

            ul {
                list-style: none;
                width: 100%;

                li {
                    @include flex(flex, row, space-between, baseline, nowrap, 0);
                    margin-bottom: 1rem;

                    i {
                        font-size: 1rem;
                        color: $primaryColor;
                    }

                }
            }

            .arrow {
                position: absolute;
                font-size: 2rem;
                top: 3%;
                right: 5%;
                display: none;
            }

            &:hover {
                margin-bottom: 1rem;

                .arrow {
                    display: block;
                }
            }
        }

        .popular {
            height: 440px;
            padding-top: 4rem;

            .ticket {
                background-color: $nex;
                color: white;
                padding: 0.3rem;
                width: 6rem;
                position: absolute;
                top: 2%;
                left: 0%;
                border-radius: 0 30px 30px 0;
            }

            &:hover {
                margin-bottom: 1rem;
            }
        }
    }
}
</style>
