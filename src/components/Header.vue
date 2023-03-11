<template>
    <div class="header">
        <div class="header__inner">
            <div class="header__block header__block--black">
                <div class="header__block__inner header__block__inner__top container">
                    <div class="header__block__left">
                        <a href="#">
                            <img class="header__logo" src="@/assets/logo.png" alt="">
                        </a>
                        
                    </div>
                    
                    <div class="header__block__right">
                        <div class="header__city">
                            <svg class="header__city__icon" width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd" d="M11 2.0625C7.57444 2.1001 4.8125 4.885 4.8125 8.31455C4.8125 8.33228 4.8125 8.35054 4.8125 8.36827C4.8125 11.7006 10.352 18.7504 10.5879 19.0485C10.6846 19.1716 10.8329 19.25 11 19.25C11.1671 19.25 11.3154 19.1716 11.4111 19.0496C11.648 18.7504 17.1875 11.7006 17.1875 8.36559C17.1875 8.35054 17.1875 8.33282 17.1875 8.31455C17.1875 4.88446 14.425 2.1001 11.0032 2.0625H11ZM11 17.8398C9.25847 15.5486 5.87107 10.624 5.87107 8.36559C5.87053 8.33873 5.86999 8.30649 5.86999 8.2748C5.86999 5.44209 8.16659 3.14605 11 3.14605C13.8334 3.14605 16.13 5.44209 16.13 8.2748C16.13 8.30649 16.1295 8.33873 16.1289 8.37042C16.1289 10.6229 12.741 15.5465 10.9995 17.8387L11 17.8398ZM11 5.64515C10.9839 5.64462 10.9651 5.64462 10.9463 5.64462C9.37346 5.64462 8.09835 6.91942 8.09835 8.49183C8.09835 10.0642 9.37346 11.339 10.9463 11.339C12.5191 11.339 13.7936 10.0648 13.7942 8.49237C13.7942 8.48485 13.7942 8.47571 13.7942 8.46658C13.7942 6.9178 12.547 5.65966 11.0016 5.64247L11 5.64515ZM11 10.2603C10.9903 10.2603 10.9785 10.2609 10.9667 10.2609C9.98926 10.2609 9.19722 9.46902 9.19722 8.49183C9.19722 7.51465 9.98926 6.7228 10.9667 6.7228C11.9441 6.7228 12.7362 7.51465 12.7362 8.49183C12.7362 8.49237 12.7362 8.49237 12.7362 8.4929C12.7362 8.49613 12.7362 8.50043 12.7362 8.50419C12.7362 9.46633 11.9608 10.248 11.0011 10.2582L11 10.2603Z" fill="#7C8792"/>
                            </svg>
                            Москва и область
                        </div>
                        <template v-if="!mobile_header">
                            <div class="header__notification">
                                <svg class="header__notification__circle" width="15" height="15" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <g clip-path="url(#clip0_404_171)">
                                        <path fill-rule="evenodd" clip-rule="evenodd" d="M5 0C2.23858 0 0 2.23858 0 5C0 7.76142 2.23858 10 5 10C7.76142 10 10 7.76142 10 5C10 2.23858 7.76142 0 5 0Z" fill="#1F2229"/>
                                        <path fill-rule="evenodd" clip-rule="evenodd" d="M5 2C6.65685 2 8 3.34315 8 5C8 6.65685 6.65685 8 5 8C3.34315 8 2 6.65685 2 5C2 3.34315 3.34315 2 5 2Z" fill="#3FCBFF"/>
                                    </g>
                                    <defs>
                                        <clipPath id="clip0_404_171">
                                            <rect width="10" height="10" fill="white"/>
                                        </clipPath>
                                    </defs>
                                </svg>

                                <svg class="header__notification__bell" width="18" height="20" viewBox="0 0 18 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" clip-rule="evenodd" d="M1.60742 0.701259C2.77891 0.0535446 4.26898 0.400996 5.01032 1.47115L5.09562 1.60302L5.73931 2.67098L5.84035 2.66333C7.98434 2.53749 10.0617 3.49113 11.2965 5.20069L11.4302 5.39374L11.5698 5.61425C12.7813 7.62379 14.1192 9.26886 15.4945 10.1813C16.1498 10.6173 16.6386 10.7787 16.8922 10.7928C17.2744 10.7596 17.619 10.9871 17.7418 11.3472C17.8545 11.6802 17.7184 12.0441 17.4293 12.2488L17.3468 12.3005L13.6194 14.3621L13.6736 14.4741C14.2988 15.8714 13.8297 17.5106 12.5501 18.4002L12.4045 18.4959L12.2525 18.5851C10.8114 19.3822 9.00558 19.045 7.96612 17.8577L7.85383 17.7223L7.76444 17.6008L4.02525 19.671C3.74961 19.8229 3.41185 19.8162 3.15412 19.6611L3.0615 19.5961L2.98593 19.5257C2.72164 19.2432 2.68786 18.8355 2.8973 18.5546C3.02502 18.3133 3.12242 17.8332 3.05715 17.0749C2.91995 15.4803 2.10277 13.5496 0.892515 11.5389C-0.295487 9.56843 -0.189833 7.14838 1.09163 5.29169L1.14277 5.21965L0.503986 4.16049C-0.151549 3.07154 0.158638 1.69806 1.1756 0.96167L1.30639 0.873006L1.4391 0.794314L1.60742 0.701259ZM3.97279 4.84428C1.82553 6.03139 1.09023 8.66969 2.32926 10.7272C3.82035 13.2022 4.63001 15.3604 4.73118 17.1471L4.737 17.2589L4.74014 17.4154L14.9574 11.7634L14.7299 11.6282C13.2457 10.7001 11.7772 9.07459 10.3564 6.79417L10.1331 6.42944C8.88949 4.36557 6.12501 3.65308 3.97279 4.84428ZM12.1656 15.1677L9.22085 16.7961L9.25416 16.8364C9.75565 17.3886 10.5931 17.5663 11.296 17.2502L11.4193 17.1882L11.5335 17.1197C12.1802 16.6987 12.4379 15.9168 12.1904 15.228L12.1656 15.1677ZM2.52696 2.05997L2.43344 2.10497L2.26636 2.19696C1.87385 2.41396 1.72199 2.8741 1.89652 3.26036L1.94263 3.34804L2.32605 3.98456L2.36689 3.95227C2.52913 3.8272 2.69875 3.70967 2.87534 3.60008L3.14541 3.44169C3.41948 3.28997 3.70327 3.15964 3.99492 3.05104L4.03138 3.03754L3.65686 2.41704C3.44708 2.06799 3.01287 1.91401 2.62327 2.02631L2.52696 2.05997Z" fill="white"/>
                                </svg>
                            </div>
                            <svg class="header__burger" @click="mobile_header = !mobile_header"  width="18" height="15" viewBox="0 0 18 15" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd" d="M0 1.5C0 0.947715 0.447715 0.5 1 0.5H17C17.5523 0.5 18 0.947715 18 1.5C18 2.05228 17.5523 2.5 17 2.5H1C0.447716 2.5 0 2.05228 0 1.5ZM0 7.5C0 6.94772 0.447715 6.5 1 6.5H17C17.5523 6.5 18 6.94772 18 7.5C18 8.05228 17.5523 8.5 17 8.5H1C0.447716 8.5 0 8.05228 0 7.5ZM1 12.5C0.447715 12.5 0 12.9477 0 13.5C0 14.0523 0.447716 14.5 1 14.5H17C17.5523 14.5 18 14.0523 18 13.5C18 12.9477 17.5523 12.5 17 12.5H1Z" fill="white"/>
                            </svg>
                        </template>
                        <template v-if="mobile_header">
                            <svg class="header__burger__close" @click="mobile_header = !mobile_header" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd" clip-rule="evenodd" d="M20.7911 3.20937C20.5142 2.93249 20.0653 2.93249 19.7884 3.20937L12 10.9978L4.21156 3.20937C3.93468 2.93249 3.48578 2.93249 3.2089 3.20937C2.93202 3.48624 2.93202 3.93515 3.2089 4.21203L10.9973 12.0005L3.2089 19.7889C2.93202 20.0658 2.93202 20.5147 3.2089 20.7916C3.48578 21.0684 3.93468 21.0684 4.21156 20.7916L12 13.0031L19.7884 20.7916C20.0653 21.0684 20.5142 21.0684 20.7911 20.7916C21.068 20.5147 21.068 20.0658 20.7911 19.7889L13.0027 12.0005L20.7911 4.21203C21.068 3.93515 21.068 3.48624 20.7911 3.20937Z" fill="white"/>
                            </svg>
                        </template>
                    </div>
                </div>
            </div>
            <div class="header__block">
                <div class="header__block__inner header__block__inner__bottom container">
                    <nav class="nav nav--desktop">
                        <div class="nav__items" ref="tabs">
                            <a 
                                class="link"
                                href="#"
                                :class="tabActive == tab.id ? 'active' : ''" 
                                v-for="tab of tabs" 
                                :key="tab.id"
                                @click="handleClickTab(tab.id)"
                            >
                                {{ tab.text }}
                            </a>
                        </div>
                        <div ref="tabline" class="nav__line"></div>
                    </nav>
                    <nav class="nav nav--mobile" :class="mobile_header ? 'open' : ''">
                        <div class="nav__items">
                            <a 
                                href="#"
                                class="link"
                                v-for="tab of tabs" 
                                :key="tab.id"

                            >
                                {{ tab.text }}
                        </a>
                        </div>
                    </nav>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'HeaderMain',
        data() {
            return {
                mobile_header: false,
                tabActive: 1,
                tabs: [
                    {
                        id: 1,
                        text: 'Преимущества Tele2'  
                    },
                    {
                        id: 2,
                        text: 'Тарифы'  
                    },
                    {
                        id: 3,
                        text: 'Акции и спецпредложения'  
                    },
                    {
                        id: 4,
                        text: 'Промотариф Tele2'  
                    },
                    {
                        id: 5,
                        text: 'Технология eSIM'  
                    },
                    {
                        id: 6,
                        text: 'Подключение нового абонента'  
                    },
                ]
            }
        },
        methods: {
            handleClickTab(id) {
                this.tabActive = id
                this.changePositionLine();
            },
            changePositionLine() {
                this.$refs.tabs.childNodes.forEach((el, index) => {
                    if (this.tabActive == index + 1) {
                        this.$refs.tabline.style.width = el.offsetWidth + "px";
                        this.$refs.tabline.style.left = el.offsetLeft + "px";
                    }

                });
            },
        },
        mounted() {
            this.changePositionLine();
        }
    }
    
</script>


<style lang="scss">
@font-face {font-family: "Tele2 TextSans Web SHORT"; src: url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.eot"); src: url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.eot?#iefix") format("embedded-opentype"), url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.woff2") format("woff2"), url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.woff") format("woff"), url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.ttf") format("truetype"), url("//db.onlinewebfonts.com/t/eaede26ebfc025d4b8715790660fbde9.svg#Tele2 TextSans Web SHORT") format("svg"); } 

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Tele2 TextSans Web SHORT';
}

a {
    text-decoration: none;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
}

.header {

    &__burger {
        display: none;
    }

    &__notification {
        display: flex;
        align-items: center;
        cursor: pointer;

        position: relative;

        &__circle {
            width: 6px;
            height: 6px;
            left: calc(50%);
            top: calc(10%);
            background: #3FCBFF;
            position: absolute;
            border-radius: 50%;
        }

    }

    &__city {
        color: #7C8792;
        margin-right: 37px;
        display: flex;
        align-items: center;
        cursor: pointer;

        &__icon {
            margin-right: 10px;
        }
    }

    &__inner {

    }

    &__block {
        

        &__inner {
            height: 40px;
            display: flex;
            align-items: center;

            &__top {
                display: flex;
                justify-content: space-between;
            }

            &__bottom {
                height: 47px;
                margin-top: 7px;
            }
        }


        &--black {
            background: #1F2229;
        }

        &__right {
            display: flex;
            align-items: center;
        }

    }
}

.nav {

    position: relative;

    &__items {
        display: flex;
        gap: 18px;
    }

    &__line {
        position: absolute;
        background: rgba(31, 34, 41, 1);
        border-radius: 2px 2px 0 0;
        height: 3px;
        left: 0px;
        bottom: 0px;
        transition: 0.3s;
    }

    &--mobile {
        display: none;

    }
    
}

.link {

    color: rgba(124, 135, 146, 1);
    font-weight: 400;
    font-size: 14px;
    cursor: pointer;
    padding-bottom: 12px;
    transition: .3s;

    &.active {
        transition: .3s;
        color: #1F2229;
    }

}

@media screen and (max-width: 1200px) {

    .container {
        padding: 0px 20px;
    }

    .nav__items { 
        max-width: 100%;
        padding-top: 30px;
    }

    .link {
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    
}

@media screen and (max-width: 768px) { 

    .header {

        &__city {
            display: none;
        }

        &__burger {
            display: block;
            margin-left: 22px;
            cursor: pointer;

            &__close {
                cursor: pointer;
            }
        }
    }

    .nav {
        
        position: fixed;
        transform: translateX(-100vw);
        transition: .3s;
        top: 40px;

        &--desktop { 
            display: none;
        }

        &--mobile {
            display: block;
            
            &.open {
                transform: translateX(0vw);
                transition: .3s;

            }

        }

        &__items {
            flex-direction: column;
            padding-top: 0px;
            text-align: start;
            gap: 16px;
            padding-top: 24px;
            width: calc(100vw - 40px);
        }

    }
    
    .link {
        justify-content: flex-start;
        padding-bottom: 0px;
        width: 100%;
        border-bottom: 1px solid #EDEDED;
        font-weight: 700;
        font-size: 16px;
        line-height: 22px;
        color: #959597;
        padding-bottom: 8px;

        &:hover {
            transition: .3s;
            color: #1F2229;
        }
    }
}



</style>1