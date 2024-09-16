<script>
export default{
    data () {
        return{
            list: [
                "caracters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop"
            ]
        }
    }
}
</script>

<template>
    <header>
        <div id="header-section" class="container">
            <img src="../assets/img/dc-logo.png" alt="logo-DC">
            <div id="list">
                <ul v-for="item in list">
                    <li>
                        {{ item }}
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped>
  header{
    height: 80px;

    #header-section{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        text-transform: uppercase;

        img{
         width: 5%;
        }

        #list{
            display: flex;

            ul{
            display: flex;

                 li{
                    font-size: 12px;
                    margin: 0.5rem;

                    &:hover{
                        color: blue;
                        cursor: pointer;
                    }
                 }
            }

        }
    }
  }
 
</style>