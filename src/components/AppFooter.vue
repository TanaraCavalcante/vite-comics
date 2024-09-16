<script>
export default{
    data () {
        return{
           
        }
    }
}
</script>

<template>
    <footer>
        <section id="shopping">
            <div class="container">
                <ul>
                    <li>
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics" >
                        digital comics
                    </li>
                    <li> 
                        <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise" >
                        dc merchandise
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="sunscription" >
                        subscription
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="shop" >
                        comic shop locator
                    </li>
                    <li>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="power visa" >
                        dc power visa
                    </li>
                </ul>
            </div>
        </section>
        <section></section>
        <section></section>
    </footer>
</template>

<style  scoped>
footer{
    color: white;

    #shopping {
        background-color: #0282F9;
        padding: 50px;
        text-transform: uppercase;
        font-size: 12px;

        ul{
            display: flex;
            justify-content: space-between;
            align-items: center;

            li{
                display: flex;
                align-items: center;
                justify-content: center;
                gap: 10px;

                img{
                width: 15%;
                }
               
            }
            
        }
    }
}
    
</style>