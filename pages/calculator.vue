<template>
<v-app>
    <v-container>
        <v-row align   ="center" justify ="center">
            <h1> Anwser :{{anwser}}  </h1>
        </v-row>
    <v-row>
        <v-col>
            <v-text-field 
                outlined 
                v-model="v1"> 
            </v-text-field>
        </v-col>
    
        <v-col>
            <v-text-field 
                outlined
                v-model="v2"> 
            </v-text-field>
        </v-col>
    </v-row>
    <v-row align   ="center" justify ="center">
        <v-btn 
            large color="green" @click="cal()">Calculator
        </v-btn>
    </v-row>
    </v-container>
</v-app>
</template>

<script>
    export default {
        data:()=>{
            return {
                v1:null,
                v2:null,
                anwser:null,
            }
        },
        computed: { //ทำงานตลอดเวลา

        },
        watch: { 

        },
        methods: { //cal หน้าที่คำนวณ v1+v2 แล้วเก็บไปที่ anwser
            cal(){
                this.anwser = parseInt(this.v1)+parseInt(this.v2)
                console.log(this.anwser);

            }
        }, 
        created () {},
    }
</script>

