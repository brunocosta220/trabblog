<script setup>
import { ref } from 'vue';
import { useRouter } from 'vue-router';
import img1 from "../assets/usuario.jpg"; // Importe a imagem aqui

const router = useRouter();
const showDropdown = ref(false);

const toggleDropdown = () => {
    showDropdown.value = !showDropdown.value;
};

const logout = () => {
    router.push('/login');
};

defineProps({
    logo: {
        type: String,
        required: true
    }
});
</script>

<template>
    <nav>
        <div id="cab">
            <div id="div_logo">
                <span>
                    <img :src="logo" >
                </span>
            </div>
        </div>
        <div id="logout-container">
            
            <span @click="toggleDropdown" id="img-options">
                <img :src="img1" alt="Opções"> <!-- Utilize :src para vincular dinamicamente a imagem -->
            </span>
            <div v-if="showDropdown" id="dropdown-menu">
                <button @click="logout">Sair</button>
               
            </div>
        </div>   
    </nav>
</template>

<style scoped>
nav {
    background-color: rgb(255, 255, 255);
    color: white;
    padding: 20px;
    right: 0px;
    width: 100%;
    position: absolute;
    top: 0px;
    display: flex;
    justify-content: space-between;
}

#img-options img{
    width: 80px;
}

#cab {
    display: flex;
    justify-content: center;
    margin-left: 20px;
}

#div_logo {
    display: flex;
    align-items: center;
    margin: auto;
}

#logout-container {
    position: relative;
}

#img-options {
    cursor: pointer;
}

#dropdown-menu {
    position: absolute;
    top: 65%;
    right: 0;
    background-color: white;
    border: 1px solid #000000;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    z-index: 1000;
    width: 120px;
    display: flex;
    flex-direction: column;
    margin-top: 20px;
}

#dropdown-menu button {
    padding: 10px;    
    width: 100%;
    text-align: left;
    background: none;
    border: none;
    cursor: pointer;
}

#dropdown-menu button:hover {
    background-color: #f0f0f0;
}
</style>
