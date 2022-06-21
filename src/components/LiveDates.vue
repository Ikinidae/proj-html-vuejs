<template>
    <section id="live_dates">
        <MusicIsLife title="Live Dates" />

        <div id="dates" class="d-flex flex-column align-items-center">
            <div class="date">
                <span @click="openClose()">&plus;</span>
                <h5>17/07/2020 GEM FESTIVAL 2020 ANAKALIA, GEORGIA</h5>

                <div ref="myDiv" class="d-none d-flex extra">
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
            <div class="date">
                <span>&plus;</span>
                <h5>24/09/2020 GROOVEFEST DOMINICAL REPUBLIC</h5>
            </div>
            <div class="date">
                <span>&plus;</span>
                <h5>31/10/2020 OASIS FESTIVAL 2020 MARRAKECH, MOROCCO</h5>
            </div>
            <div class="date">
                <span>&plus;</span>
                <h5>07/11/2020 MOGA FESTIVAL - ESSAOURIA, MOROCCO</h5>
            </div>
            <div class="date">
                <span>&plus;</span>
                <h5>10/12/2020 ENVISION FESTIVAL - UVITA, COSTA RICA</h5>
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
            showMore: false

        }
    },
    methods: {
        openClose() {
            if (this.$refs.myDiv.classList[0]==="d-none") {
                this.$refs.myDiv.remove("d-none");
                this.$refs.myDiv.add("d-block");
            } else {
                this.$refs.myDiv.add("d-none");
            }
            // if (this.showMore == false) {
            //     this.showMore == true;
            // } else {
            //     this.showMore == false;
            // }
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#live_dates {
    background-color: #252a33;

    #dates {

        // width: 80%;
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