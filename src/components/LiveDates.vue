<template>
    <section id="live_dates">
        <MusicIsLife title="Live Dates" />

        <div id="dates" class="d-flex flex-column align-items-center">
            <div class="date" v-for="(item, i) in dates" :key="i">
                <span @click="changeActive(item)">&plus;</span>
                <h5>{{ item.name }}</h5>

                <div v-if="item.active" class="d-flex extra">
                    <div>
                        <img src="../assets/map.png" alt="">
                    </div>
                    <div class="extra_info">
                        <h4>Untold Stories</h4>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nesciunt recusandae adipisci non
                            eius, culpa eaque, doloremque suscipit, debitis soluta voluptate necessitatibus voluptatibus
                            dolorum sed exercitationem.</p>
                        <a href="">BOOK NOW</a>
                    </div>
                </div>
            </div>
        </div>

        <p id="all_latest_news">
            VIEW ALL LIVE DATES
        </p>
    </section>
</template>

<script>
import MusicIsLife from './MusicIsLife.vue';

export default {
    name: 'LiveDates',
    components: {
        MusicIsLife
    },
    data() {
        return {
            dates: [
                {
                    name: "17/07/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA",
                    active: false
                },
                {
                    name: "24/09/2020 GROOVEFEST DOMINICAL REPUBLIC",
                    active: false
                },
                {
                    name: "31/10/2020 OASIS FESTIVAL 2020 MARRAKECH, MOROCCO",
                    active: false
                },
                {
                    name: "07/11/2020 MOGA FESTIVAL - ESSAOURIA, MOROCCO",
                    active: false
                },
                {
                    name: "10/12/2020 ENVISION FESTIVAL - UVITA, COSTA RICA",
                    active: false
                }
            ],
            showMore: false
        }
    },
    methods: {
        changeActive(item) {
            if (item.active === false) {
                item.active = true;
            } else {
                item.active = false;
            }
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#live_dates {
    background-color: #252a33;

    #dates {
        .date {
            background-color: #323844;
            width: 65%;
            margin: 4px;
            padding: 5px 20px;

            span {
                color: white;
                margin-right: 20px;
                cursor: pointer;
            }

            h5 {
                color: #ea4a56;
                display: inline-block;
                font-size: 12px;
                font-weight: bolder;
                margin: 0;
            }

            .extra {
                margin: 20px 20px 20px 5px;

                img {
                    width: 300px;
                }

                .extra_info {
                    margin-top: 25px;
                    margin-left: 30px;

                    h4 {
                        font-size: 15px;
                        color: white;
                        margin-bottom: 15px;
                    }

                    p {
                        font-size: 13px;
                        color: #aeaeaf;
                        margin-bottom: 30px;
                    }

                    a {
                        color: white;
                        background-color: #ea4a56;
                        font-size: 13px;
                        text-decoration: none;
                        padding: 8px 15px;
                    }
                }
            }
        }
    }

    #all_latest_news {
        background-color: #eb4b54;
        width: 100%;
        text-align: center;
        margin-top: 30px;
        padding-top: 30px;
        padding-bottom: 30px;
        color: white;
        font-size: 12px;
        font-weight: bolder;
        cursor: pointer;
        margin-bottom: 0;

        &:hover {
            color: black;
            background-color: white;
        }
    }
}
</style>