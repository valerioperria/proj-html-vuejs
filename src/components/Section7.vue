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
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="wrapper">
            <h5><strong>SEND A MESSAGE</strong></h5>
            <h1><strong>Get in</strong><strong class="touch">Touch</strong></h1>
            <p>We will respond to your message as soon as possible.</p>
            <div class="inputs">
                <input type="text" id="name" placeholder="Name">
                <input type="email" id="mail" placeholder="Email">
                <input type="text" id="phone" placeholder="Phone">
                <select id="info" placeholder="More Info">
                    <option>More Info</option>
                </select>
                <textarea id="message" cols="30" rows="10" placeholder="Message"></textarea>
            </div>
            <button>SEND</button>
        </div>
        <div class="example">
            <h2><strong>Example inc.</strong></h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
            <p>Deleniti placeat similique cumque deserunt molestias rerum soluta quaerat vitae optio.</p>
            <div class="contact" v-for="item in contacts"><i :class="item.icon"></i>
                <span>{{ item.text }}</span>
            </div>
            <button>VIEW MAP</button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;
@use "../style/partials/mixin" as *;

.container {
    width: 100%;
    padding: 120px 350px;
    @include flex(flex, row, baseline, baseline, nowrap, 0);

    .wrapper {
        width: 60%;

        h5 {
            color: $nex;
            margin-bottom: 2rem;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;
        }

        .touch {
            background-color: $primaryBg;
            color: $primaryColor;
            padding: 0.5rem;
            margin-left: 0.5rem;
            border-radius: 6px;
        }

        p {
            margin-bottom: 3rem;
        }

        .inputs {
            @include flex(flex, row, baseline, baseline, wrap, 1rem);
            border: none;
            margin-bottom: 1rem;

            input,
            select,
            textarea {
                padding: 0.7rem;
                width: calc((100% / 2) - 1rem);
                border: none;
                background-color: rgba(0, 0, 0, 0.13);
                border-radius: 4px;
                color: gray;
            }

            #message {
                width: calc(100% - 1rem);
                height: 140px;
            }

            #name {
                background-image: url(../assets/img/image.png);
                background-repeat: no-repeat;
                background-position-x: 98%;
                background-position-y: center
            }
        }

        button {
            @include button;
            margin-left: 0;
        }
    }

    .example {
        width: 40%;
        padding: 1rem 1rem 1rem 2rem;
        @include flex(flex, column, baseline, baseline, wrap, 1.5rem);

        .contact {
            i {
                color: $primaryColor;
                font-size: 1rem;
                background-color: $primaryBg;
                width: 40px;
                height: 40px;
                line-height: 40px;
                border-radius: 50%;
                text-align: center;
                margin-right: 0.7rem;
            }

            span {
                font-size: 1.2rem;
                color: $primaryColor;
            }
        }

        button {
            @include darkButton;
            color: $primaryColor;

            &:hover {
                color: white;
            }
        }
    }
}</style>
