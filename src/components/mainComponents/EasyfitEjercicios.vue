<template>
    <div class="container-fluid">
        <div class="row">
            <local-nav class="container-fluid col-sm-1 p-0 m-0" :data="local_nav_data"></local-nav>
            <router-view class="col-sm-11"></router-view>
        </div>
    </div>
</template>

<script>
import LocalNavigator from './LocalNavigator.vue';

export default {
    name: 'EasyfitEjercicios',

    components: {
        'local-nav': LocalNavigator,
    },

    data: function() {
        return {
            local_nav_data: [
                {
                    title: 'Introducción',
                    subtitles: [],
                    link: '/ejercicios'
                },
                {
                    title: 'Fuerza',
                    subtitles: [],
                    link: '/fuerza'
                },
                {
                    title: 'Explosividad',
                    subtitles: [],
                    link: '/explosividad'
                },
                {
                    title: 'Resistencia',
                    subtitles: [],
                    link: '/resistencia'
                }
            ]
        };
    }
};
</script>