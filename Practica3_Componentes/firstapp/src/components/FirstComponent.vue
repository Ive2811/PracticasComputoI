<template>
   <div id="root">
       <h1 v-on:mousemove="getXY">{{title}}</h1>
       {{x}},{{y}}
       </div> 
</template>

<script>
export default{
    name:'FirstComponent',
    data(){
        return{
            title: 'Mi primer componente',
            x:0,
            y:0
        }
        },
        methods:{
            getXY(event){
                this.x=event.offsetX;
                this.y=event.offsetY;
            }
        }
     }

</script>
