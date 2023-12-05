<script>
export default {
    data() {
        return {
            company: [
                {
                    icon: "fa-brands fa-google-scholar",
                    name: "Tradition",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-lock",
                    name: "Security",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-pen-to-square",
                    name: "Certificate",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
                {
                    icon: "fa-solid fa-graduation-cap",
                    name: "Expertise",
                    text: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
                },
            ]
        };
    },
}
</script>

<template>
    <div class="container">
        <svg class="svgUp" width="150" height="100">
            <defs>
                <pattern width="150" height="100" id="dotted-texture" patternContentUnits="userSpaceOnUse"
                    patternUnits="userSpaceOnUse" fill="rgba(13, 128, 130, 0.232)">
                    <g id="row-1">
                        <ellipse cx="5" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                    <g id="row-2">
                        <ellipse cx="5" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                    <g id="row-3">
                        <ellipse cx="5" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                    <g id="row-4">
                        <ellipse cx="5" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                </pattern>
            </defs>
            <rect width="150" height="100" x="0" y="0" fill="url(#dotted-texture)"></rect>
        </svg>
        <div class="wrapper">
            <h5><strong>ABOUT THE NETWORK</strong></h5>
            <h1><strong class="the">The</strong><strong>Company</strong></h1>
            <p>For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related
                services to select clients.</p>
            <ul>
                <li v-for=" item in company">
                    <div class="list">
                        <i :class="item.icon"></i>
                        <h3>{{ item.name }}</h3>
                    </div>

                    <p>{{ item.text }}</p>
                </li>
            </ul>
        </div>
        <div class="img"></div>
        <svg class="svgDown" width="150" height="100">
            <defs>
                <pattern width="150" height="100" id="dotted-texture" patternContentUnits="userSpaceOnUse"
                    patternUnits="userSpaceOnUse" fill="rgba(13, 128, 130, 0.232)">
                    <g id="row-1">
                        <ellipse cx="5" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="5" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                    <g id="row-2">
                        <ellipse cx="5" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="20" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="35" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="50" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="65" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="80" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="95" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="110" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="125" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                        <ellipse cx="140" cy="20" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    </g>
                    <g id="row-3">
                        <ellipse cx="5" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="20" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="35" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="50" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="65" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="80" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="95" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="110" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="125" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="140" cy="35" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                </g>
                <g id="row-4">
                    <ellipse cx="5" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="20" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="35" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="50" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="65" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="80" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="95" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="110" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="125" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                    <ellipse cx="140" cy="50" rx="3" ry="3" style="stroke:none;stroke-width:0"></ellipse>
                </g>
            </pattern>
        </defs>
        <rect width="150" height="100" x="0" y="0" fill="url(#dotted-texture)"></rect>
    </svg>
</div></template>

<style lang="scss" scoped>@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    height: 800px;
    @include flex(flex, row, center, center, nowrap, 0);
    position: relative;

    .svgUp {
        position: absolute;
        top: -3.5%;
        right: 45.8%;
    }

    .svgDown {
        position: absolute;
        bottom: -9.1%;
        right: 45.8%;
    }

    .wrapper {
        height: 100%;
        width: 50%;
        @include flex(flex, column, center, baseline, nowrap, 0);
        padding: 0 26px 0 350px;

        h5 {
            margin-bottom: 2rem;
            color: $nex;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;

            .the {
                color: $primaryColor;
                background-color: $primaryBg;
                padding: 0.5rem;
                margin-right: 0.5rem;
                border-radius: 6px;
            }
        }

        p {
            margin-bottom: 4rem;
        }

        ul {
            @include flex(flex, row, space-between, center, wrap, 1rem);

            li {
                width: calc(50% - 1rem);
                list-style: none;

                .list {
                    @include flex(flex, row, baseline, center, wrap, 8px);
                    margin-bottom: 1rem;

                    i {
                        color: $primaryColor;
                        font-size: 1.5rem;
                    }
                }

                p {
                    margin-bottom: 2rem;
                }
            }

        }
    }

    .img {
        height: 100%;
        width: 50%;
        background-image: url(../assets/img/about-3.jpg);
        background-size: cover;
    }
}</style>
