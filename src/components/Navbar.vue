<template>
    <div class="navbar">
        <div class="_container">
            <div class="navbar__wrapper">
                <div class="navbar__block-1">
                    <div class="logo">
                        <img src="@/assets/logo.png" alt="" >
                    </div>
                    <div class="navbar__rout">
                        <span>Blog</span>
                        <span>FAQ</span>
                        <span>Reviews</span>
                        <span>Contact us</span>    
                    </div>
                </div>
                <div class="navbar__block-2">
                    <div class="searchbar">
                        <div class="hand-bag-icon"></div>
                        <form-block class="form-block" style="widht:100%">
                            <div class="form-block__wrapper">
                                <input type="text" placeholder="Search" class="Search">
                                <div class="search-icon"></div>
                            </div>
                        </form-block>
                        <div class="language-buttons">
                            <form-block  class="form-block-2">
                                <a href="#" class="language-button language-active">US</a>
                                <a href="#" class="language-button">EU</a>
                            </form-block>
                        </div>
                    </div>
                </div>
            </div>
            <div class="navbar__wrapper-2">
                 <div class="language-buttons">
                    <form-block  class="form-block-2">
                        <a href="#" class="language-button language-active">US</a>
                        <a href="#" class="language-button">EU</a>
                    </form-block>
                </div>
                <div class="logo">
                    <img src="@/assets/logo.png" alt="" >
                </div>
                <div class="navbar__wrapper-2__icons">
                    <div class="hand-bag-icon"></div>
                    <div class="burger-menu"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default{
}

</script>

<style lang="scss" scoped>
    .navbar{
        background: rgba(20, 20, 20, 0.12);
        height: 15vh;
        max-height: 71px;
        display: flex;
        align-items: center;
        @media(max-width: 770px){
            max-height: 100px;
        }
        @media(max-width: 500px){
            max-height: 84px;
        }
    }
    .logo{
        height: 39px;
        width: 54px;
        img{
            object-fit: fill;
        }
    }
    .navbar__rout{
        margin-left: 35px;
        span{
            margin-left: 29px;
            font-family: 'Inter';
            font-style: normal;
            font-weight: 500;
            font-size: 14px;
            line-height: 127.2%;
            letter-spacing: -0.025em;
            color: #FFFFFF;
        }
        span:first-child{
            margin-left: 0px;
        }
    }
    .navbar__wrapper{
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 100%;
        @media(max-width: 770px){
            flex-wrap: wrap;
            justify-content: center;
        }
        @media(max-width: 500px){
            display: none;
        }
        .navbar__block-1{
            display: flex;
            align-items: center;
            flex:1 1 49%;
            @media(max-width: 770px){
                justify-content: center;
            }
        }
        .navbar_block-2{
            flex:1 1 49%;
            margin: 0 auto;
            @media(max-width: 770px){
                flex-wrap: wrap;
                padding-top:10px
            }
        }
    }
    ._container{
        max-width: 1110px;
        overflow: hidden;
        margin: 0 auto;
        width: 100%;
        padding: 0 20px;
        @media(max-width:340px){
            padding: 0 10px;
        }
    }
    .form-block{
        display: flex;
        justify-content: center;
        align-items: center;

        .form-block__wrapper{
            display: flex;
            align-items: center;
            margin: 0 auto;
            width: 90%;
            height:35px;
            justify-content: space-between;
            .Search{
                background: none;
                border: none;
                font-family: 'Inter';
                font-style: normal;
                font-weight: 400;
                font-size: 0.875rem ;
                line-height: 127.2%;
                letter-spacing: -0.025em;
                color: #757575;
                width: 90%;
            }
            .search-icon{
                background-image: url(@/assets/MagnifyingGlass.svg);
                width: 16px;
                height: 16px;
                background-size: contain;
                background-repeat: no-repeat;
                background-position: center center;
            }
        }
    }

    .searchbar{
        display: flex;
        align-items: center;

        .hand-bag-icon{
            height: 20px;
            width: 20px;
            background: url(@/assets/Handbag.svg);
            background-size:contain;
            background-repeat: no-repeat;
            background-position: center center;
            margin-right: 13px;

        }
    }
    .form-block-2{
        display: flex;
        align-items: center;
        justify-content: center;
        margin-left: 11px;
        padding: 0 5px;
        .language-button{
            text-decoration: none;
            font-family: 'Quarion';
            font-style: normal;
            font-weight: 700;
            font-size: 1rem;
            line-height: 127.2%;
            letter-spacing: -0.025em;
            color: #F1433A;
        }
        .language-button:nth-child(2){
            margin-left: 12px;
        }
        .language-active{
            font-family: 'Quarion';
            font-style: normal;
            font-weight: 400;
            font-size: 1rem;
            line-height: 127.2%;
            letter-spacing: -0.025em;
            color: #757575;
        }
    }
    .navbar__wrapper-2{
        align-items: center;
        justify-content: space-between;
        display: none;
        @media(max-width: 500px){
            display: flex;
        }
    }
    .navbar__wrapper-2__icons{
        display: flex;
        align-items: center;
        .hand-bag-icon{
            height: 20px;
            width: 20px;
            background: url(@/assets/Handbag.svg);
            background-size:contain;
            background-repeat: no-repeat;
            background-position: center center;
            margin-right: 13px;
        }
        .burger-menu{
            height: 20px;
            width: 20px;
            background: url(@/assets/TextAlignRight.svg);
            background-size:contain;
            background-repeat: no-repeat;
            background-position: center center;
            margin-right: 13px;
        }
    }
</style>