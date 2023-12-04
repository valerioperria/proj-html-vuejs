<script>
export default {
    data() {
        return {
            openHours: [{
                icon: "fa-regular fa-clock",
                text: "Open Hours: Mon - Sat - 9:00-18:00"
            },],
            contacts: [{
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
        };
    },
}
</script>

<template>
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

    </section>
</template>

<style lang="scss" scoped>
@use "../style/partials/variables" as *;

#lineUp {
    width: 100%;
    height: 50px;
    background-color: $bgLineUp;
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: $textLineUp;

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
</style>
