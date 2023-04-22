<template>
<v-app>
<v-container><!--ตีกรอบหน้าไว้จัดหน้า -->
    <v-row align   ="center" justify ="center"> <!--จัดระเบียงให้มันอยู่กึ่งกลาง -->
     <v-btn rounded > <!--ปุ่มเป็นวงรี -->
        
       <v-icon>mdi-account-circle</v-icon> 
        Hello !!
     </v-btn>  <!-- สร้างปุ่ม -->
     <v-btn color="red"> <!-- สร้างสีปุ่ม -->
        I am Mayjaree
     </v-btn>
    </v-row>
     
    <v-row><!-- สร้างให้กรอก user /outlined แบบมีกรอบ--> 
        <v-text-field 
            outlined 
            label="User ID"
        ></v-text-field>
    </v-row>
      
    <v-row> <!-- สร้างให้กรอก password /outlined แบบมีกรอบ--> 
        <v-text-field 
            outlined            
            label="Password"
            type ="password"   
        ></v-text-field>
    </v-row>
    
    <v-row align   ="center" justify ="center">
        <v-btn>
            login
        </v-btn>

    </v-row>
</v-container>
</v-app>
</template>
<script>
    export default {
        data:()=>{

        },
        computed: {         //มีหน้าที่ทำงานตลอดเวลา 

        }, 
        watch: {            //ดูข้อมูลการเปลี่ยนแปลงทั้งหมด



        },  
        methods: {      //ใช้สำหรับสร้างฟังก์ชั่นต่างๆ



        }, 
        created () {         //ทุกครั้งที่เปิดหน้าweb runcode




        }, 
    }
</script>