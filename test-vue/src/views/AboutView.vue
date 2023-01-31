<template>
    <div class="about">
        <h1>회원가입 추가 정보 입력</h1>
        <h1>{{ type }} 사용자입니다</h1>
        <h1>{{ userId }}</h1>
        <h1>{{ nickname }}</h1>
        <h1>{{ email }}</h1>
        <img :src="profile" alt="" />
    </div>
</template>

<script>
export default {
    name: "test-test",
    data() {
        return {
            nickname: "",
            userId: "",
            profile: "",
            email: "",
            type: "",
        };
    },
    created() {
        this.nickname = new URL(window.location.href).searchParams.get("nickname");
        this.userId = new URL(window.location.href).searchParams.get("userId");
        this.profile = new URL(window.location.href).searchParams.get("profile");
        this.email = new URL(window.location.href).searchParams.get("email");
        this.type = new URL(window.location.href).searchParams.get("type");
    },
};
</script>
