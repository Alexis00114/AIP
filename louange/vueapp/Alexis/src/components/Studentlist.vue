<template>
    <div class="table-container">
        <h2>List of students</h2>
        <table border="1">
            <tr>
                <th>ID</th>
                <th>Name</th>
                <th>Level</th>
                <th>Trade</th>
                </tr>
            <tr v-for="data in student" :key="data.id">
            <td>{{data.id}}</td>
            <td>{{data.name}}</td>
            <td>{{data.level}}</td>
            <td>{{data.trade}}</td>
            

            </tr>
        </table>
    </div>
    <div><p>We have many students but those aaaare Examples o</p>
        <h1>REGTRATION FORM</h1>
        <P>Login to your account</P>
    </div>

</template>
<script>
export default {
    data(){
        return{
            student: [
                {id:1,name:"ALEXIS",level:4,trade:"SWD"},
                {id:2,name:"LUOANGE",level:3,trade:"SWD"},
                {id:3,name:"MANZI",level:5,trade:"SWD"},
                {id:3,name:"MANZI",level:5,trade:"SWD"},
                {id:3,name:"MANZI",level:5,trade:"SWD"},
                {id:3,name:"MANZI",level:5,trade:"SWD"},
                {id:4,name:"DOXA",level:3,trade:"SWD"}
            ]

        }
    }
}
</script>