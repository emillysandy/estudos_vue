# ESTUDANDO VUE #
 Esse repositório tem como objetivo copilar os meus estudos relacionados aos estudos de Vue.

 ### Vue.js: o meio termo ###
 Um arquivo ".vue" possui 3 seções:
  1. Template: o código HTML.
  2. Script: a lógica do componente com código Javascript/Typescript.
  3. Style: o estilo do componente, em que as definições podem ser limitadas ao escopo.
 O que for definido no Script pode ser utilizado no template para manipular o DOM, e vice-versa.

 ### Exemplo: componente de botão com Vue ###
   Similar ao Angular, um componente pode receber propriedades (props como no React) usando diretivas.
  Entretanto, no Vue temos sintaxes menores como os dois pontos ":" que permite atribuir valores dinâmicos a
  propriedades/atributos. No caso dos eventos, podemos usar o arroba "@" e para uma função ser executada temos
  elementos especiais que podem ser usados para manipulação, como o "slot", que tal como o "ng-content", faz a
  projeção do conteúdo passado dentro do componente quando usado. A configuração é feita dentro do "script", exportando
  um objeto com alguns atributos, como "name" e "props".

```
  <template>
  <button :title="titulo" @click="aoClicar">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "Botao",
  props: {
    titulo: String,
    aoClicar: Function,
  },
};
</script>

<style>
</style>
```
