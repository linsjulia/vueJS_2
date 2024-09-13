<template>
    <section>
        <div>
            <p>Meu conteudo</p>
            <div>
                <input v-model="name" placeholder="Digite seu nome">
                <p>Seu nome é: {{ name }}</p>
                <button @click="submeterFormulario()" >Procurar usuário</button>
            </div>
        </div>
    </section>
</template>

<script>



export default {
    name: 'ContentPage',
    data() {
        return {
            name: '',
            url: ''
        }
    },
    methods: {
        submeterFormulario(){
            fetch(`https://api.github.com/users/${this.name}`)
            .then((data) => {
                this.url = data.url
                console.log(data.url);

        });
            
        }
    }
}
</script>

<style></style>