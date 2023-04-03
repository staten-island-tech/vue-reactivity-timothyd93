<template>
    <div id="list">
        <li> {{ name }}</li>
    </div>
</template>

<script>
export default {
    name:"List",
    props: {
        name: String,
    }
}
</script>