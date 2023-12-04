<script>
export default {
    data() {
        return {
            openHours: [
                {
                    icon: "fa-solid fa-clock",
                    text: "Open Hours: Mon - Sat - 9:00-18:00"
                },
            ],
            contacts: [
                {
                    icon: "fa-solid fa-phone",
                    text: "+1 (305) 1234-5678"
                },
                {
                    icon: "fa-solid fa-envelope",
                    text: "hello@example.com"
                },
                {
                    icon: "fa-brands fa-facebook",
                },
                {
                    icon: "fa-brands fa-twitter",
                },
                {
                    icon: "fa-brands fa-linkedin-in",
                },
            ],
            menu: [
                { title: "HOME" },
                { title: "ABOUT" },
                { title: "SERVICES" },
                { title: "PRICING" },
                { title: "BLOG" },
            ]
        };
    },
}
</script>

<template>
    <div class="container">
        <section id="lineUp">
            <div class="openHours" v-for="item in openHours">
                <i :class="item.icon"></i>
                <span>{{ item.text }}</span>
            </div>
            <div class="contacts">
                <div class="contact" v-for="item in contacts"><i :class="item.icon"></i>
                    <span>{{ item.text }}</span>
                </div>
            </div>
        </section>
        <section id="hero">
            <div class="logoAndMenu">
                <div class="logo">
                    <h3 class="nex">N E X</h3>
                    <h3 class="gen">G E N</h3>
                </div>
                <div class="menu">
                    <ul>
                        <li v-for="item in menu"><strong>{{ item.title }}</strong></li>
                    </ul>
                    <button><strong>GET IN TOUCH</strong></button>
                </div>
            </div>
            <div class="title">
                <h1><strong>Lead ~ </strong><strong class="costumer">Customer</strong></h1>
                <p>Successfull strategies require data analysis, creativity and customer focus, taking advantage of the
                    latest
                    technologies to offer excellent services.</p>
                <div class="buttons">
                    <button class="get"><strong>GET IN TOUCH</strong></button>
                    <button class="read"><strong>READ MORE</strong></button>
                </div>

            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    background-image: url(../assets/img/hero-image.png);
    background-size: cover;

    #lineUp {
        width: 100%;
        height: 50px;
        background-color: $bgLineUp;
        @include flex(flex, row, space-between, center, nowrap, 0);
        color: $textLineUp;
        padding: 0 350px;

        i {
            margin-right: 6px;
        }

        .contacts {
            display: flex;

            .contact {
                margin-left: 1rem;
            }
        }
    }

    #hero {
        width: 100%;
        height: 850px;
        padding: 0 350px;
        @include flex(flex, column, base-line, base-line, no-wrap, 0);
        background-color: rgba(0, 0, 0, 0.641);

        .logoAndMenu {
            @include flex(flex, row, space-between, base-line, no-wrap, 0);
            margin: 2rem 0;

            .logo {
                @include flex(flex, row, baseline, center, wrap, 4px);

                .nex {
                    color: $nex;
                    background-color: rgba(13, 128, 130, 0.402);
                    padding: 0.5rem 0.2rem 0.5rem 1rem;
                    border-radius: 18px 0 0 18px
                }

                .gen {
                    color: $textLineUp;
                }
            }

            .menu {
                display: flex;
                align-items: center;
                color: white;

                ul {
                    display: flex;
                    list-style: none;

                    li {
                        margin-left: 1rem
                    }
                }

                button {
                    @include button;
                }
            }
        }

        .title {
            @include flex(flex, column, baseline, center, wrap, 2rem);
            height: 100%;
            color: white;
            padding-top: 13rem;

            h1 {
                font-size: 4rem;

                .costumer {
                    background-color: rgba(13, 128, 130, 0.232);
                    padding: 0 0.5rem;
                }
            }

            p {
                max-width: 650px;
            }

            .buttons {
                @include flex(flex, row, baseline, baseline, wrap, 1rem);

                .get {
                    @include button;
                }

                .read {
                    @include darkButton;
                }
            }
        }
    }
}</style>
