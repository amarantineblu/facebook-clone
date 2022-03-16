<template>
    <BreezeAuthenticatedLayout>
        <div class="col-lg-6">
            <div class="central-meta">
                <div class="groups">
                    <span><i class="fa fa-users"></i> Users </span>
                </div>
                <ul class="nearby-contct">
                    <li v-for="user in users" :key="user.id">
                        <div class="nearly-pepls">
                            <figure>
                                <a href="time-line.html" title=""><img src="images/resources/group1.jpg" alt=""></a>
                            </figure>
                            <div class="pepl-info">
                                <h4><a href="time-line.html" title="">{{user.name}}</a></h4>
                                <span>{{user.username}}</span>
                                <em>32k Members</em>
                                <a href="#" title="" class="add-butn" data-ripple=""> follow</a>
                            </div>
                        </div>
                    </li>

                </ul>87
            </div><!-- photos -->
        </div>

    </BreezeAuthenticatedLayout>
</template>

<script setup>
    import BreezeAuthenticatedLayout from '@/Layouts/Authenticated.vue';
    defineProps({
        users: ''
    })

</script>

<style lang="scss" scoped>

</style>
//
