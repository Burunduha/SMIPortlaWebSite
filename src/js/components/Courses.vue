<template >
    <div class="courses">
        <div class="courses-item">
            <img src="/img/swift.jpg" alt="SMI portal">
            <h4>Front-end</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. In, distinctio deserunt?</p>
            <button>ДЕТАЛИ</button>
        </div>
        <div class="courses-item">
            <img src="/img/swift.jpg" alt="SMI portal">
            <h4>Swift</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. In, distinctio deserunt?</p>
            <button>ДЕТАЛИ</button>
        </div>
        <div class="courses-item">
            <img src="/img/swift.jpg" alt="SMI portal">
            <h4>Python</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. In, distinctio deserunt?</p>
            <button>ДЕТАЛИ</button>
        </div>
        <div class="courses-item">
            <img src="/img/swift.jpg" alt="SMI portal">
            <h4>Angular</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. In, distinctio deserunt?</p>
            <button>ДЕТАЛИ</button>
        </div>
        <div class="courses-item">
            <img src="/img/swift.jpg" alt="SMI portal">
            <h4>PHP & MySQL</h4>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. In, distinctio deserunt?</p>
            <button>ДЕТАЛИ</button>
        </div>
    </div>
</template>

<script>

</script>

<style lang="scss" scoped>
    .courses {
    margin-bottom: 25px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    @media (min-width: 555px) {
        justify-content: space-between;
        
        }
    @media (max-width: 555px) {
        justify-content: center;
        flex-direction: column;
        align-items: center;
        }
    
    
    .courses-item {
        margin-top: 70px;
        
        position: relative;
        overflow: hidden;

        h4 {
            color: #000;
            margin-bottom: 20px;
        }

        p {
            max-width: 250px;
        }

        img {
            width: 200px;
            height: 120px;
            transition: all 0.5s ease;
            &:hover {
                box-shadow: #000 0px 0px 16px;
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

</style>