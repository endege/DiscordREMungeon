<template>
    <div>
        <p>You aren't in the Discord REMungeon guild! Please join to use this panel:</p>
        <a href="https://none">https://none</a>
    </div>
</template>

<script>
    export default {
        created() {
            // Set $route values that are not preset during unit testing
            if (process.env.NODE_ENV === 'testing') {
                this.$route = {
                    name: 'panel',
                    path: '/panel'
                };
            }
        }
    };
</script>

<style scoped>
    code {
        background-color: rgba(40, 56, 76, .5);
        border-radius: 3px;
        color: #fff;
        font-weight: bold;
        padding: 3px 6px;
        margin: 0 3px;
        vertical-align: bottom;
    }
    
    .full {
        width: 100%;
    }
    
    p {
        line-height: 24px;
    }
</style>
