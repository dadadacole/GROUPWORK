<template>
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
        <span class="navbar-brand ps-2">TodoList App</span>
        <button class="navbar-toggler" type="button" @click="isNavShow = !isNavShow">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div :class="isNavShow ? 'collapse navbar-collapse show' : 'collapse navbar-collapse'">
            <ul class="navbar-nav">
                <li class="nav-item">
                    <router-link class="nav-link" to="/"> Home </router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" to="/CardRecommendation"> 카드 추천 </router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" to="/InOut">InOut</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" to="/Listview">회원가입/로그인</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" to="/Challenge">무지출 챌린지</router-link>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script setup>
import { ref } from 'vue';

const isNavShow = ref(false);
</script>
