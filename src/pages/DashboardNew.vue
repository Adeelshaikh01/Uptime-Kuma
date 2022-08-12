<template>
    <div class="container-fluid">
        <div class="row">
             <div class="col-12  position-sticky fixed-top ">
                <router-view :key="$route.fullPath" />
            </div>

            <div class="col-12">
                <MonitorListNew :scrollbar="true" />
            </div>

        </div>
    </div>
</template>

<script>

import MonitorListNew from "../components/MonitorListNew.vue";

export default {
    components: {
        MonitorListNew,
    },
    data() {
        return {};
    },
};
</script>

<style lang="scss" scoped>
@import "../assets/vars.scss";
.container-fluid {
    width: 98%;
}
</style>