<template>
    <div class="home">
        <h1>{{ userId }}</h1>
    </div>
</template>

<script>
export default {
    name: "HomeView",
    components: {},
    data() {
        return {
            userId: "",
        };
    },
    created() {
        this.memberId = new URL(window.location.href).searchParams.get("userId");
    },
};
</script>
