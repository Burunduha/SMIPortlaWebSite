<template >
    <div class="popular-article">
        <div class="lead">
            <div>
                <h1>Работа мечты <br> компания Google</h1>
                <p class="question">что из себя представляет работа в google</p>
                <p>Для многих людей Google представляется большим зданием с прозрачными лоджиями и окнами от пола до потолка, которое усеяно уютными и красивыми креслами/столами. От представления кафетерия в этом здании, мечты становятся ещё красочнее, еда пестрит излишествами и деликатесами и всё это бесплатно. В окружении только доброжелательные, невероятно умные и весёлые коллеги-друзья. Что же здесь правда?</p>
                <button>ЧИТАТЬ ДАЛЕЕ</button>
            </div>
            <div>
                <img src="/img/canteen.jpeg" alt="SMI portal">
            </div>
        </div>
    </div>
</template>
<script>

</script>

<style lang="scss" scoped>
.popular-article{
    margin-top: 50px; 
    margin-bottom: 20px;
    padding-bottom: 60px;
    border-bottom: 1px #ABABAB solid;
    .lead{
        display: flex;
        
        justify-content: space-between;
        flex-wrap: wrap-reverse;


        
        .question {
            margin-top: 20px;
            margin-bottom: 40px;
            text-transform: uppercase;       
        }
        h1 {
            color: #303030;
        }
        p{
            @media (min-width:600px){
            width: 600px;
            }
        }
        button {
            border: 2px #2477ca solid ;
            color: #2477ca;
            background: #fff;
            font-size: 0.9em;
            font-weight: 600;
            padding: 10px 20px;
            margin-top: 30px;
            cursor: pointer;
            transition: background-color 0.5s ease;

            &:hover {
            background-color: #b8d9fa;
            }
        }
        >div:last-of-type {
            img {
                @media (min-width: 640px) {
                    width: 576px;
                }
                @media (max-width: 640px) {
                    width: 290px;
                }
                
                
                border: 0;
                border-radius: 2%;
            }
        }
    }
}
</style>