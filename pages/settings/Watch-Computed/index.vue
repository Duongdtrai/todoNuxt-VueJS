<template>
    <div>
        <h1>Watch-Computed</h1>
        <div v-for="(number,index) in numbers" :key = "index">
            <li>
                {{number}}
            </li>
        </div>

    </div>
</template>

<script>
export default {
    name: 'IndexPage',
    data () {
        return {
            isShow: false,
            student: [
                'Vũ Thanh Anh',
                'Đậu Văn Lạc',
                'Nguyễn Văn Chiến',
                'Bành Thị Nở',
                'Trần Thanh Cảnh',
            ],
            AllNumber: [
                1,2,3,4,5,6,7,8,9,10
            ],
        };
    },
    watch: {
        newTodoText(toOld,toNew) {
            console.log(toOld);
            // console.log(new1);
        },
    },
    computed:{
        numbers(){
            return this.AllNumber.filter((value,index) => {
                return value%2 === 0
            })
        }
    },
}





// computed: khi dùng computed thì nó phải return trong 1 hàm, khi nào biến trong hàm được thay đổi thì thực hiện, chỉ cần cái tên hàm là cái như biến được sử dụng, bên trong là sự thay đổi của các biến tùy vào trong hàm
// watch: không cần trả về, nó chỉ có tác dụng là xem old và new 
</script>

