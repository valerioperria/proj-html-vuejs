<script>
export default {
    data() {
        return {
            cards: [
                {
                    icon: "fa-solid fa-network-wired",
                    name: "Audit & Assurance",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-coins",
                    name: "Financial Dvisory",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-chart-simple",
                    name: "Analytics and M&A",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-plane-departure",
                    name: "Middle Marketing",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-scale-balanced",
                    name: "Legal Consulting",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-inbox",
                    name: "Regulatory Risk",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
            ]
        };
    },
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <h5><strong>OUR BUSINESS AREAS</strong></h5>
            <h1><strong>Excellence in</strong><strong class="services">Services</strong></h1>
            <div class="pEButton">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of
                    experienced and renowned professionals. These are some options that you can hire.</p>
                <button>SEE ALL</button>
            </div>
        </div>
        <div class="cards">
            <ul>
                <li v-for=" item in cards">
                    <i :class="item.icon"></i>
                    <h2>{{ item.name }}</h2>
                    <p>{{ item.text }}</p>
                    <button>READ MORE</button>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    height: 1100px;
    padding: 120px 350px;
    background-color: rgb(24, 24, 29);

    .wrapper {
        margin-bottom: 2rem;

        h5 {
            color: $nex;
            margin-bottom: 2rem;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;
            color: white;

            .services {
                background-color: $primaryBg;
                padding: 0.5rem;
                margin-left: 0.5rem;
                border-radius: 6px;
            }
        }

        .pEButton {
            @include flex(flex, row, space-between, center, nowrap, 0);

            p {
                color: white
            }

            button {
                @include darkButton;
                width: 8rem;
                margin-left: 200px;
            }
        }
    }

    .cards {
        ul {
            @include flex(flex, row, space-between, center, wrap, 1.5rem);

            li {
                @include flex(flex, column, baseline, baseline, wrap, 1.5rem);
                color: white;
                width: calc((100% / 3) - 1.5rem);
                list-style: none;
                background-color: rgb(31, 31, 36);
                padding: 2rem;
                border-radius: 12px;
                margin-top: 1rem;

                i {
                    color: $nex;
                    font-size: 2rem;
                }

                p {
                    max-width: 80%;
                }

                button {
                    @include darkButtonNoHover;
                }

                &:hover {
                    margin-top: 0;

                    i{
                        color: white;
                    }

                    button {
                        border-color: rgb(0, 164, 164);
                        background-color: rgb(0, 164, 164);
                    }
                }
            }
        }
    }
}
</style>
