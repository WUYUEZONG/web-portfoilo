<template>
  <div class="board">
    <div>
        <img src="@/assets/Spense.png" alt="" />
    </div>
    <div>
        <span class="title">Spense.com</span>
        <!-- <img src="/src/assets/Social Icons/LinkedIn.svg" alt="" /> -->
    </div>
    <div>
        <span class="detail">
            Rethinking the way writers get paid, an open-source platform designed to help writers focus more on writing, and less on <i>when</i> and <i>how</i> they'll get paid. Project in collaboration with Codewell.cc
        </span>
    </div>
  </div>
</template>

<style scoped>
.board {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.board img {
    width: 100%;
}
.board {
    max-width: 490px;
    width: 45%;
}



.board .title {
    font-size: 2rem;
}
.detail {
    line-height: 1.6rem;
}

@media (max-width: 767px) {
    .board, .board img {
    max-width: 100%;
    width: 100%;
}
}

</style>