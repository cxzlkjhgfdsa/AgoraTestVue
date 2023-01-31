<template>
    <div class="home">
        <h1>Social Login</h1>
        <br />
        <a href="http://localhost:8080/oauth2/authorization/google">
            <h1>구글 로그인</h1>
        </a>
        <br />
        <a href="http://localhost:8080/oauth2/authorization/naver">
            <h1>네이버로그인</h1>
        </a>
        <br />
        <a href="http://localhost:8080/oauth2/authorization/kakao">
            <h1>카카오로그인</h1>
        </a>
    </div>
</template>

<script>
export default {
    name: "HomeView",
    components: {},
};
</script>
