<template>
    <div>
        <wx-search
            v-model="searchContent1">
        </wx-search>
        <div class="result m-b-20">
            <text class="f32">{{searchContent1}}</text>
        </div>

        <wx-search
            v-model="searchContent2"
            placeholder="请输入"
            :autofocus="true"
            bgColor="#4676FF"
            innerBgColor="#fff"
            cancelColor="#fff">
        </wx-search>
        <div class="result m-b-20">
            <text class="f32">{{searchContent2}}</text>
        </div>
    </div>
</template>

<script>
    import WxSearch from '../../packages/wx-search/index'

    export default {
        data () {
            return {
                searchContent1: '',
                searchContent2: ''
            }
        },

        methods: {

        },

        components: {WxSearch}
    }
</script>
<style scoped>
    .result {
        width: 750px;
        height: 40px;
    }
    .m-b-20 {
        margin-bottom: 20px;
    }
    .f32 {
        font-size: 32px;
    }
</style>
