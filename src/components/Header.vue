<template>
    <div class="board">
        <h2 class="title">Johnathan Specter</h2>
        <ul>
            <li v-for="i in lists" :key="i">
                <span>{{ i }}</span>
            </li>
        </ul>
        <span>
            <button>Get in touch</button>
            <img src="@/assets/HamburgerMenu.svg" alt="" />
        </span>
    </div>
</template>

<script setup>
const lists = ['Articles', 'Chats', 'Awards', 'About']
</script>

<style scoped>
.board {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

ul {
    list-style: none;
    display: flex;
    gap: 20px;
}

img {
    display: none;
}

@media (max-width: 767px) {

    ul,
    button {
        display: none;
    }

    img {
        display: block;
    }
}
</style>