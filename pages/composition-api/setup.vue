<template>
  <div>
    <!--    <p>{{fullName}}</p>-->
    <p>{{message}}</p>
  </div>
</template>

<script lang="ts">
    import {createComponent, computed, ref} from '@vue/composition-api'

    interface User {
        firstName: string
        lastName: number
    }



    export default {
        setup() {
            // const user: User = {
            //     firstName: "Gene",
            //     lastName: 123,
            // };
            // const fullName = computed(() => `${user.firstName} ${user.lastName}`)
            const message = ref('This is a message');

            return {
                // fullName,
                message
            }
        }
    }
</script>
