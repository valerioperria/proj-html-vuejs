<script>
export default {
    data() {
        return {
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
                    icon: "fa-solid fa-location-dot",
                    text: "Main Avenue, 987"
                },
            ],
            cards: [
                {
                    title: "About",
                    list: [
                        { name: "The Company" },
                        { name: "Institutional" },
                        { name: "Social & Events" },
                        { name: "Innovation" },
                        { name: "Enviroment" },
                        { name: "Technology" },
                    ]
                },
                {
                    title: "Services",
                    list: [
                        { name: "Audit & Assurance" },
                        { name: "Financial Advisoy" },
                        { name: "Analytics M&A" },
                        { name: "Middle Marketing" },
                        { name: "Legal Consulting" },
                        { name: "Regulatory Risk" },
                    ]
                },
                {
                    title: "Support",
                    list: [
                        { name: "Responsibility" },
                        { name: "Terms of Usa" },
                        { name: "About Cookies" },
                        { name: "Privacy Policy" },
                        { name: "Accessibility" },
                        { name: "Information" },
                    ]
                }
            ]
        };
    },
}
</script>

<template>
    <div class="container">
        <section id="footer">
            <div class="logoAndOthers">
                <div class="logo">
                    <h3 class="nex">N E X</h3>
                    <h3 class="gen">G E N</h3>
                </div>
                <div class="others">
                    <p>A Functional HTML Template for Corporate & Business.</p>
                    <div class="contact" v-for="item in contacts"><i :class="item.icon"></i>
                        <span>{{ item.text }}</span>
                    </div>
                    <button>GET IN TOUCH</button>
                </div>
            </div>
            <div class="card" v-for="item in cards">
                <h2>{{ item.title }}</h2>
                <ul v-for="obj in item.list">
                    <li><i class="fa-solid fa-chevron-right"></i>{{ obj.name }}</li>
                </ul>
            </div>
        </section>
    </div>
    <section id="lineDown">
        <p>Enloy the low price. We are tracking any intention of privacy.</p>
        <p><i class="fa-regular fa-copyright"></i>2020 NEXGEN is Proudly Powered by <span>Codings</span></p>
        <button><i class="fa-solid fa-arrow-up"></i></button>
    </section>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    padding: 120px 350px;
    background-color: rgb(24, 24, 29);

    #footer {
        @include flex(flex, row, space-between, center, wrap, 2rem);

        .logoAndOthers {
            padding: 1rem 1rem 1rem 0;

            .logo {
                @include flex(flex, row, baseline, center, wrap, 4px);
                margin-bottom: 1.5rem;

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

            .others {
                color: white;

                p {
                    margin-bottom: 1.5rem;
                }

                .contact {
                    margin-bottom: 1rem;

                    i {
                        margin-right: 6px;
                    }
                }

                button {
                    @include darkButton;
                    margin-top: 1.5rem;
                }
            }
        }

        .logoAndOthers,
        .card {
            width: calc((100% / 4) - 2rem);
            height: 100%;
        }

        .card {
            padding: 2rem;
            background-color: rgba(255, 255, 255, 0.077);
            border-radius: 12px;
            color: white;
            padding: 1rem;

            h2 {
                margin-bottom: 1rem;
            }

            ul {
                list-style: none;

                i {
                    margin-right: 1rem;
                }

                li {
                    margin-bottom: 0.7rem;
                }
            }

        }
    }
}

#lineDown {
    width: 100%;
    height: 50px;
    background-color: black;
    @include flex(flex, row, space-between, center, nowrap, 0);
    color: white;
    padding: 0 350px;
    font-size: 0.7rem;
    position: relative;

    p {
        i {
            margin-right: 4px;
        }

        span {
            color: $primaryColor;
        }
    }

    button {
        background-color: black;
        border: none;
        position: absolute;
        right: 1%;

        i {
            color: black;
            font-size: 1.5rem;
            background-color: rgba(255, 255, 255, 0.05);
            width: 30px;
            height: 30px;
            line-height: 30px;
            border-radius: 50%;
            text-align: center;
        }
    }
}</style>
