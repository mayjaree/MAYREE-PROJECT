<template> <!--สร้างหน้า login--> 
   <v-app>
        <v-row align   ="center" justify ="center"><!--สร้างกึ่งกลางหน้าจอ--> 
            <VCard align   ="center" justify ="center" width="400"><!--สร้างlogin ให้อยู่ในcard-->
                <v-card-text>
                <v-row align   ="center" justify ="center">
                    <h1 >Login Home </h1><!--สร้างtext ข้อความหัวข้อ-->
                </v-row>
                <v-row>
                    <v-text-field outlined label="User ID"></v-text-field> <!--สร้างข้อความที่พิมไรก็ได้ /outlinedใส่กรอบ-->
                </v-row>
                <v-row>
                    <v-text-field outlined label="password" type="password"></v-text-field><!--สร้างข้อความให้เป๊น password-->
                </v-row>
                <v-row align   ="center" justify ="center">
                    <v-btn large color="red">Login</v-btn><!--สร้างปุ่มlogin-->
                    <v-btn large color="green">reset</v-btn>
                </v-row> 

            </v-card-text>
            </VCard>
        </v-row>
    </v-app>
</template>

<script>


</script>