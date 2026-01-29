<template>
    <section>
        <div class="container text-light py-5">
            <div class="text w-100 text-end fs-6">
                <h3>
                    DECEMBER / 2025 <br>
                    BRIGITTE SCHWARTZ
                </h3>
            </div>
            <div class="text text-uppercase w-100 text-start mt-3">
                <h2>
                    <span class="firstName">
                        nhoem
                    </span>
                    <span class="lastName">
                        senkropum
                    </span>
                </h2>
            </div>
            <div class="text d-flex justify-content-between">
                <div class="desc text-start">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Praesentium et fugit quas voluptatibus exercitationem asperiores autem. Dolorem mollitia eligendi sint dicta ullam iste, quisquam quos deleniti. Ea eos magni quaerat?</div>
                <div class="desc text-end">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores ullam nostrum quisquam cum quis sed pariatur iste. Aperiam nisi pariatur id nulla consequatur nostrum, repellendus odio impedit, ea qui possimus?</div>
            </div>
        </div>
    </section>
    <section>
        <div class="container d-flex gap-2">
            <div v-for="btn in myBtns" class="allBtns">
                <BaseBtn :title="btn"/>
            </div>
        </div>
    </section>
</template>
<style scoped>
.firstName{
    line-height: 1;
    margin: 0;
    font-size: 6rem;
}
.lastName{
    line-height: 1;
    margin: 0;
    font-size: 22rem;
}
.desc{
    font-size: 1.5rem;
    width: 35%;
}
</style>

<script setup>
import BaseBtn from '@/component/buttons/BaseBtn.vue';
import { reactive } from 'vue';



let myBtns =  reactive([
    'Introduction',
    'Experience',
    'Skills',
    'Education'
])
</script>