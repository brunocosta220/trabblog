<script setup>
defineProps({
  titulo: {
    type: String,
    required: true
  },
  txt: {
    type: String,
    required: true
  },
  post: {
        type: String,
        required: true
    }
})
</script>

<template>
    <nav>
        <div id="cab">
            <div id="div_logo">
                <span>
                    <img :src="post">
                </span>
            </div>
            <div id="div_titulo">
                <span>{{ titulo }}</span>
            </div>
            <div id="div_txt">
                <span>{{ txt }}</span>
            </div>
        </div>
    </nav>
</template>

<style scoped>
.div_titulo{
    color: red;
    font-size: larger;
}
</style>