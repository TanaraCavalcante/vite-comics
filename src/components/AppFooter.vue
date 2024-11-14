<script>
export default{
    data () {
        return{
           content: [
            {
                title:"DC COMICS",
                listItem: [     //content[i].listItem[i]
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
           links:[
            "digital comics",
            "dc merchandise",
            "subscription",
            "comic shop locator",
            "dc power visa"
           ]
        //    social:[
        //         "facebook",
        //         "twitter",
        //         "youtube",
        //         "pinterest",
        //         "periscope"
        //    ],
        }
    },
    
}
</script>

<template>
    <footer>
        <section id="shop">
            <div class="container">
                <ul>
                    <li v-for="link in links">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                        <a href="#">{{ link }}</a>
                    </li>
                    
                </ul>
            </div>
        </section>
        <section id="info">
            <div  id="DC-links">
                <ul>
                    <li v-for="(item, index) in content" :key="index">{{ item.title }}
                      <p v-for="(elemento, index) in item.listItem" :key="index">{{elemento}} </p> 
                    </li>
                </ul>
            </div>
            <div>
                <img src="../assets/img/dc-logo-bg.png" alt="dc.bg">
            </div>
            
        </section>
        <section id="follow">
            <div class="container">
                 <button>SIGN-UP NOW!</button>
                 <div >
                    <h4>FOLLOW-US</h4>
                    <div id="links" >
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

<style lang="scss" scoped>
footer{
    color: white;

    #shop {
        background-color: #0282F9;
        padding: 50px;
        text-transform: uppercase;
        font-size: 12px;
        z-index: 1;

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
        height: 300px;
        display: flex;
        
        position: relative;
        

          #DC-links{
            display: flex;
            flex-direction: column;
            gap: 5px;
            margin-bottom: 10px;

          }
          img{
            width: 25%;
            position: absolute; 
            top: -20px;
            right: 280px;
          }
    }
    #follow {
        background-color: #303030;
        padding: 30px;
        position: sticky;
     

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