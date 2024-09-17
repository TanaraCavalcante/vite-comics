<script>
export default{
    data () {
        return{
           content: [
            {
                title:"DC COMICS",
                listItem: [
                    "Caracters",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ],
            },
            {
                title:"SHOP",
                 listItem: [
                    "Shop DC",
                    "Shop DC Collextibles",                  
                ],
            },
            {
                title:"DC",
                 listItem: [
                    "Terms of use",
                    "Privacy policy (Nex)",
                    "Ad Choices",
                    "Adversing",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshops",
                    "CPSC Certificates",
                    "Ratings",
                    "Shop Help",
                    "Contact Us"
                ]
            },
            {
                title:"Sites",
                 listItem: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa" 
                ]
            }
           ],
        }
    }
}
</script>

<template>
    <footer>
        <section id="shop">
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
        <section id="info">
            <div v-for="item in content" class="container">
                <h4>{{ item.title }}</h4>
                <ul>
                    <li>
                        <a href="#"></a>
                    </li>
                </ul>
            </div>
        </section>
        <section id="follow">
            <div class="container">
                 <button>SIGN-UP NOW!</button>
                 <div >
                    <h4>FOLLOW-US</h4>
                    <div id="links">
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt="Facebook"></a>
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt="Twiter"></a>
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>  
                    </div>    
                 </div>
            </div>
        </section>
    </footer>
</template>

<style  scoped>
footer{
    color: white;

    #shop {
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
    #info {
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        padding: 30px;
        height: 400px;
        
        
    }
    #follow {
        background-color: #303030;
        padding: 30px;

        div {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        div button {
            background-color: #303030;
            padding:15px;
            border: 2px solid  #0282F9;
            color: white;

                &:hover{
                        color: #0282F9;
                        cursor: pointer;
                        }
        }

        h4{
            color: #0282F9;
            margin-right: 10px;
        }

        #links {
            display: flex;
            gap: 10px;  
        }
    }
}   
</style>