<template >
    <div class="last-published">
        <div class="last-published-heading">
            <h2>Последние опубликованные</h2>
        </div>
        <div class="last-published-articles">
            <table>
                <tbody>
                    <tr>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                        <td>
                            <img src="img/maxresdefault.jpg" alt="SMI portal">
                            <h3>Какие языки программирования ненавидят больше и почему?</h3>
                            <p>Авторитетный веб-ресурс Stack Overflow решил заняться опросом в отношении языков программирования. В этот раз в центре внимания нелюбимые языки.</p>
                            <button>ДАЛЕЕ</button>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss" scoped>
    .last-published {
        
        .last-published-articles{
            padding-bottom: 60px;
            margin-bottom: 20px;
            border-bottom: 1px #ababab solid;

            table {
                border-collapse: collapse;
                tr {
                    
                    &:first-child td {
                        border-top: none;
                    }
                    &:last-child td {
                        border-bottom: none;
                    }

                    td {
                        border: 1px solid #ababab;
                        
                        border-left: 0;
                        @media (min-width: 570px) {
                            padding: 40px;
                        }
                        @media (max-width: 570px) {
                            padding: 10px;
                        }
                        p {
                            @media (min-width: 570px) {
                            font-size: 1em;
                        }
                        @media (max-width: 570px) {
                            font-size: 0.7em;
                        }
                        }
                        
                        &:last-of-type{border-right: 0;}
                        h3 {
                            color: #000;
                            margin: 20px 0;
                            @media (min-width: 570px) {
                            font-size: 1.3em;
                        }
                        @media (max-width: 570px) {
                            font-size: 0.8em;
                        }
                        }

                        img {
                        
                        width: 95%;
                        
                        border: 1px #000 solid;
                        border-radius: 2%;
                        transition: all 0.5s ease;
                        

                        &:hover {
                            border-radius: 0;
                            transform: scale(1.05);
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
                }
                    
                }
            }
        }
    }
</style>