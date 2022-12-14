<template>
    <div>
        <form>
            <div>
                <label for="Name">Name:</label>
                <input type="text" v-model="Name"> <br/>
                <label for="Surname">Surname:</label>
                <input type="text" v-model="Surname">
            </div>
            <label for="email">Email:</label>
            <input type="text" v-model="Email">
            <label for="PhoneNumber">Phone Number:</label>
            <input type="number" v-model="PhoneNumber">
            <input type="submit" id="submit" placeholder="Submit" :placeholder="Submit" v-on:click.prevent="submit">

        </form>
    </div>
</template>
<script>
export default {
    name: 'Contact'
}
</script>
<style>
    
</style>