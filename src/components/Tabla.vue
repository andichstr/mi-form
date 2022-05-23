<template>
    <div class="container">
        <table class="table">
            <thead>
                <tr>
                    <th>#</th>
                    <th>Nombre</th>
                    <th>Edad</th>
                    <th>Email</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(item, i) in usuarios" :key="item.id">
                    <td>{{i}}</td>
                    <td>{{item.nombre}}</td>
                    <td>{{item.edad}}</td>
                    <td>{{item.email}}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    props: {
        usuarios: {
            type: Array,
            required: true,
        }
    }
}
</script>

<style>

</style>