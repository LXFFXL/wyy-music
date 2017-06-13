<template>
    <div >
        <tabbar>
            <tabbar-item selected>
                <img slot="icon" :src="tabbar[0].icon" />>
                <img slot="icon-active" :src="tabbar[0].iconActive"/>>
                <span slot="label">{{tabbar[0].label}}</span>
            </tabbar-item>
            <tabbar-item>
                <img slot="icon" :src="tabbar[1].icon" />>
                <img slot="icon-active" :src="tabbar[1].iconActive"/>>
                <span slot="label">{{tabbar[1].label}}</span>
            </tabbar-item>
            <tabbar-item>
                <img slot="icon" :src="tabbar[2].icon" />>
                <img slot="icon-active" :src="tabbar[2].iconActive"/>>
                <span slot="label">{{tabbar[2].label}}</span>
            </tabbar-item>
            <tabbar-item>
                <img slot="icon" :src="tabbar[3].icon" />>
                <img slot="icon-active" :src="tabbar[3].iconActive"/>>
                <span slot="label">{{tabbar[3].label}}</span>
            </tabbar-item>
        </tabbar>
    </div>
</template>

<script>
import { Tabbar, TabbarItem } from 'vux'
export default {
    components: {
        Tabbar,
        TabbarItem,
    },
    data () {
        return {
            tabbar: [
                {
                    icon: require('../assets/tabbar/cm2_btm_icn_discovery@3x.png'),
                    iconActive: require('../assets/tabbar/cm2_btm_icn_discovery_prs@3x.png'),
                    label: '发现音乐'
                },
                {
                    icon: require('../assets/tabbar/cm2_btm_icn_music@3x.png'),
                    iconActive: require('../assets/tabbar/cm2_btm_icn_music_prs@3x.png'),
                    label: '我的音乐'
                },
                {
                    icon: require('../assets/tabbar/cm2_btm_icn_friend@3x.png'),
                    iconActive: require('../assets/tabbar/cm2_btm_icn_friend_prs@3x.png'),
                    label: '朋友'
                },
                {
                    icon: require('../assets/tabbar/cm2_btm_icn_account@3x.png'),
                    iconActive: require('../assets/tabbar/cm2_btm_icn_account_prs@3x.png'),
                    label: '账号'
                },
            ],
            tabbarSelected: 1,
        }
    }
}
</script>

<style scoped>

</style>