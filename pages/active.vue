<template>
    <div>
        <IndexAction></IndexAction>
    </div>
</template>

<script>
import IndexAction from './index/action';

export default {
    layout: 'index',
    name: 'Active',
    data() {
        return {
            pageItem: '1'
        }
    },
    components: {
        IndexAction
    },
    methods: {
        handleSelect(val) {
            console.log(val)
            this.pageItem = val;
        }
    }
}
</script>
<style lang="less">

</style>
