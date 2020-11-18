<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-header">Example Component</div>

                    <div class="card-body">
                        {{showExample}}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['propito'],
        computed: {
            showExample(){
                return this.propito;
            }
        },
        mounted() {
            console.log('Component mounted.')
            console.log(this.propito)
        },
        created(){
            console.log(this.propito)
        }
    }
</script>
