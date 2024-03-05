<script>
    export default {
        data: () => ({
            Contador: 0,
        }),
        methods: {
            incrementar () {
                this.Contador++;
            },
            disminuir(){
                this.Contador--;
            },
            multi (){
                this.Contador *=2;
            },
            divi (){
                this.Contador /=2;
            },
            reset () {
                this.Contador = 0;
            },
        },
    };        
</script>

<template>
    <div class="container">
        <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
        <small>
            <h1>VUE.C</h1>
        </small>
        <hr />

        <h2>Contador: {{ Contador }}</h2>
        <button @click="incrementar()">+1</button>
        <button @click="disminuir()">-1</button>    
        <button @click="multi()">*2</button>
        <button @click="divi()">/2</button>
        <button @click="reset()">Resetear</button>
    </div> 
</template>

<style scoped>

.container {
text-align: center;
}

small {
    color: rgb(226, 68, 11);
}

h1 {
    font-weight: bolder;
    font-size: 3.5rem;
    margin: 8px;
}
h2 {
    font-size: 2.5rem;
}
button {
    cursor: pointer;
    font-size: 1.5rem;
    margin: auto;
}
</style>

