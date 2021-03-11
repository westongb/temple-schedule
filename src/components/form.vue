<template>
    <form>
        <h3> Pick your Time</h3>
        <div class="name">
            <label>Family Name</label>
            <input type="text">
        </div>
        <label for="example-datepicker">Choose a date and time</label>

            <select>
            <option v-for="item in dates" :key="item.date" :value="item.date"> {{item.date}}</option>
            </select>
                <select>
            <option v-for="item in times" :key="item" :value="item"> {{item}}</option>
            </select>
            </form>
</template>

<script>
import { defineComponent } from '@vue/composition-api'


export default defineComponent({
    setup() {
        
    },
    data(){
            return {
                value: '',
                dates: [{date: "4-10-2021"},{date: "4-17-2021"}],
                times: ['5:20','5:40','6:00','6:20','6:40' ]
            }
        }
})
</script>

<style scoped>
 form{
     margin-top: 150px;
 }
 .name{
     margin: 5% 5% 5% 5%;
 }
 label{
     margin: 0 2% 0 1%;
 }
</style>