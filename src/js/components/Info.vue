<template >
    <div class="info">
        <div class="info-heading">
            <h5>Информация</h5>
        </div>
        <div class="info-content">
            <i v-if="screenWidth > 770" class="fa-solid fa-people-group"></i>
            <div class="info-content-item">
                <i v-if="screenWidth <= 770" class="fa-solid fa-people-group"></i>
                <h6>Множество клиентов</h6>
                <p>Огромное количество клиентов выбирают нас, так как мы всегда держим руку на пульсе всего происходящего</p>
            </div>
            <i v-if="screenWidth > 770" class="fa-brands fa-youtube"></i>
            <div class="info-content-item">
                <i v-if="screenWidth <= 770" class="fa-solid fa-people-group"></i>
                <h6>Большая аудитория YouTube</h6>
                <p>Большая фан база на площадке YouTube. Вы всегда сможете найти ту информацию, которая сейчас у всех на слуху на нашем канале</p>
            </div>
        </div>
    </div>
</template>

<script>
export default{
   data(){
    return {
        screenWidth: screen.width,
    }
   },
   mounted(){
    this.onScreenResize();
   },
   methods: {
        onScreenResize(){
            window.addEventListener('resize', () => {
                this.screenWidth = screen.width
            })
        }
        }
   }
</script>

<style lang="scss" scoped>
    .info {
        margin-bottom: 60px;
        i {
                    color: #2477ca;
                    font-size: 3em;
                    line-height: 2em;
                }
        .info-heading {
            max-width: 200px;
            border-bottom: 3px #2477ca solid;
            padding-bottom: 10px;
            margin-bottom: 60px;
            h5 {
                color: #000;
                font-size: 1.7em;
            }
        }
        .info-content {
            display: flex;
            justify-content: space-around;
            @media (max-width: 770px) {
                flex-wrap: wrap;
            }
            .info-content-item {
                position: relative;
                h6 {
                    font-size: 1.2em;
                    color: #000;
                    margin-bottom: 20px;
                }
                p {
                    max-width: 520px;
                }
                
            }
        }
    }
</style>