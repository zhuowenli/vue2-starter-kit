<template lang="jade">
    header.header
        .container.flex
            h1.flex__item
                router-link(to="/") LOGO
            el-tabs
                el-tab-pane(label="控制中心")
                el-tab-pane(label="用户管理")
                el-tab-pane(label="权限管理")
</template>

<style lang="scss">
    @import "../stylesheets/common";

    .header{
        height: 80px;
        background: $blue;
        @include user-select(none);
        h1{
            line-height: 80px;
            font-size: 32px;
            font-weight: 400;
            a{
                display: block;
                color: #fff;
            }
        }
        .el-tabs{
            &__header{
                border: 0;
            }
            &__item{
                height: 80px;
                line-height: 80px;
                opacity: .8;
                color: #fff;
                font-size: 16px;
                @include transition(opacity 0.1s ease-in-out);
                &.is-active, &:hover{
                    opacity: 1;
                }
            }
            &__active-bar{
                background: $light-blue;
                height: 4px;
            }
        }
    }
</style>