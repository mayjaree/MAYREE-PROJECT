<template>
    <v-app>
        <v-data-table         
           :headers="headers"  
           :items="desserts"
        >
            <template v-slot:item.calories="{ item }">
                <v-chip
                    :color=getcolor(item.calories)
                    dark
                >
                    {{ item.calories }}
                </v-chip>
            </template>
        </v-data-table> <!-- เก็บข้อมูลtableตามตัวแปร -->
    </v-app>
</template> 

    <script>
        export default {
            data:()=>{
            return {
                headers: [     //ชื่อตัวแปรheaders หัวข้อด้านบน
                { text: 'name' , value: 'name'}, // text ตามด้วยชื่อหัวข้อของคอลัม value คือค่าตัวแปรที่ใช้แสดงผลของข้อมูลนั้น
                { text: 'Calories', value: 'calories' },
                { text: 'Fat (g)', value: 'fat' },
                { text: 'Carbs (g)', value: 'carbs' },
                { text: 'Protein (g)', value: 'protein' },
                { text: 'Iron (%)', value: 'iron' },
                         ],

                desserts: [   //<--ชื่อตัวแปรdesserts ข้อมูลที่ต้องการเก็บตามaray
          {
            name: 'Frozen Yogurt',
            calories: 159,
            fat: 6.0,
            carbs: 24,
            protein: 4.0,
            iron: 1,
          },
          {
            name: 'Ice cream sandwich',
            calories: 237,
            fat: 9.0,
            carbs: 37,
            protein: 4.3,
            iron: 1,
          },
          {
            name: 'Eclair',
            calories: 262,
            fat: 16.0,
            carbs: 23,
            protein: 6.0,
            iron: 7,
          },
          {
            name: 'Cupcake',
            calories: 305,
            fat: 3.7,
            carbs: 67,
            protein: 4.3,
            iron: 8,
          },
          {
            name: 'Gingerbread',
            calories: 356,
            fat: 16.0,
            carbs: 49,
            protein: 3.9,
            iron: 16,
          },
          {
            name: 'Jelly bean',
            calories: 375,
            fat: 0.0,
            carbs: 94,
            protein: 0.0,
            iron: 0,
          },
          {
            name: 'Lollipop',
            calories: 392,
            fat: 0.2,
            carbs: 98,
            protein: 0,
            iron: 2,
          },
          {
            name: 'Honeycomb',
            calories: 408,
            fat: 3.2,
            carbs: 87,
            protein: 6.5,
            iron: 45,
          },
          {
            name: 'Donut',
            calories: 452,
            fat: 25.0,
            carbs: 51,
            protein: 4.9,
            iron: 22,
          },
          {
            name: 'KitKat',
            calories: 518,
            fat: 26.0,
            carbs: 65,
            protein: 7,
            iron: 6,
          },
                         ]
                }
        },
            computed: {         //มีหน้าที่ทำงานตลอดเวลา 

            }, 
            watch: {            //ดูข้อมูลการเปลี่ยนแปลงทั้งหมด

            },  
            methods: {      //ใช้สำหรับสร้างฟังก์ชั่นต่างๆ 
                getcolor(calories){
                    if(calories<200){
                        return "green"
                    }
                    else if(calories<350){
                        return "blue"
                    }
                    else{ 
                        return "red"
                    }
                }, 
            }, 
            created () {}       //ทุกครั้งที่เปิดหน้าweb runcode
        
        }
    </script>