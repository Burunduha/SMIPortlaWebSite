<template>
    <nav :class="[ { 'nav-active': isNavOpen }]">
        <div class="menu-button" @click="toggleNav">
            <i class="fa-solid fa-bars"></i>
        </div>
        <div class="menu">
            <div class="search-block">
                <input class="nav-menu-search" type="search" placeholder="Поиск">
            </div>
            <div class="nav-menu">
                <div class="nav-menu-heading">
                    <h4>Меню</h4>
                </div>
                <ul>
                    <li><a href="">ГЛАВНАЯ</a></li>
                    <li><a href="">ПРО НАС</a></li>
                    <li><a href="">КОНТАКТЫ</a></li>
                </ul>
            </div>
            <div class="about-us">
                <div class="about-us-heading">
                    <h4>Информация про нас</h4>
                </div>
                <div class="about-us-content">
                    <div class="about-us-content-item">
                        <img src="img/macbookhackcode.jpg" alt="SMI portal">
                        <p>На днях был придуман новый язык программирования - Kotik!</p>
                    </div>
                    <div class="about-us-content-item">
                        <img src="img/macbookhackcode.jpg" alt="SMI portal">
                        <p>Эксперты усомнились в подлинности данных, которые предоставила компания Apple</p>
                        <button>ДАЛЕЕ</button>
                    </div>
                </div>
            </div>
            <div class="help">
                <div class="help-heading"> 
                    <h4>Помощь</h4>
                </div>
                <div class="help-content">
                    <p>Если у вас возникли какие-либо вопросы и вы хотите связаться с нами для уточнения всех моментов, то ниже представлены все контактные данные для связи с нами.</p>
                    <ul>
                        <li><a href="mailto:test@itproger.com"><i class="fa-regular fa-envelope"></i>test@itproger.com</a></li>
                        <li><a href="tel:0000000000"><i class="fa-solid fa-phone"></i>(000) 000-0000</a></li>
                        <li><adress><i class="fa-solid fa-house"></i>USA Washington Seatle Northway 13002</adress></li>
                    </ul>
                </div>
            </div>
            <div class="menu-footer">Все права защищены ©. При использовании данных указывайте ссылку на первоисточник</div>
        </div>
    </nav>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isNavOpen: false
      };
    },
    methods: {
      toggleNav() {
        this.isNavOpen = !this.isNavOpen;
      }
    }
  };
  </script>
  
  <style lang="scss">
  nav {
    
    position: fixed;
    width: 250px;
    height: 100%;
    background: #ececec;
    left: -250px;
    transition: all 0.5s ease;
    
    .menu-button {
        position: absolute;
        left: 270px;
        top: 20px;
        color: #2477ca;
        cursor: pointer;

        &:hover {
            color: #003264;
        }
    }
    .menu{
        height: calc(100% - 40px);
        overflow-y: auto;
       
        
        &::-webkit-scrollbar {
            width: 8px;
        }

        &::-webkit-scrollbar-thumb {
            background-color: #c4c4c4;
            border-radius: 4px;
        }

        &::-webkit-scrollbar-thumb:hover {
            background-color: #a0a0a0;
        }

        &::-webkit-scrollbar-button {
            display: none;
        }
        .search-block{
            padding: 10px;
            padding-left: 30px;
            background: #e7e7e7;
            .nav-menu-search {
                padding: 4px 0 4px 12px;
                outline: none;
                border: 0;
                border-radius: 4%;
                &::placeholder {
                    color: #a0a0a0;
                }
            }
        }
        .nav-menu {
            .nav-menu-heading {
                margin-top: 30px;
                width: 25%;
                color: #000;
                padding-bottom: 10px;
                margin-left: 15px;
                border-bottom: #2477ca solid 2px;
            }
            ul {
                margin: 30px 20px 0 20px;
                list-style: none;
                
                li {
                    padding-bottom: 15px;
                    margin-bottom: 20px;
                    border-bottom: #ababab solid 1px;
                    a {
                        color: #949494;
                        font-weight: 600;
                        transition: color 0.5s ease;
                        &:hover {
                            color: #666666;
                        }
                    }
                }
            }
        }
        .about-us {
            margin: 50px 0 0 0;
            .about-us-heading { 
                margin-top: 30px;
                width: 75%;
                color: #000;
                padding-bottom: 10px;
                margin-left: 15px;
                border-bottom: #2477ca solid 2px;
            }
            .about-us-content {
                padding: 15px;
                margin-top: 20px;
                .about-us-content-item {
                    border-bottom: #ababab solid 1px;
                    margin-bottom: 20px;
                    img {
                        width: 210px;
                        height: 80px;
                        border: 0;
                        border-radius: 3%;
                        opacity: 90%;
                        transition: all 0.5s ease;

                        &:hover {
                            opacity: 100%;
                            transform: scale(1.05);
                            border-radius: 0%;
                        }
                    }
                    p {
                        font-size: 0.7em;
                        margin: 10px 0 30px 0;
                    }
                    button {
                        border: 2px #2477ca solid ;
                        color: #2477ca;
                        background: #ececec;
                        font-size: 0.9em;
                        font-weight: 600;
                        padding: 10px 20px;
                        margin-bottom: 10px;
                        cursor: pointer;
                        transition: background-color 0.5s ease;

                        &:hover {
                        background-color: #b8d9fa;
                        }
                    }
                }
            }
        }
        .help {
            .help-heading {
                width: 32%;
                color: #000;
                padding-bottom: 10px;
                margin-left: 15px;
                border-bottom: #2477ca solid 2px;
            }
            .help-content {
                p {
                    margin-top: 10px;
                    padding: 15px;
                    font-size: 0.7em;
                }
                ul {
                margin: 30px 20px 0 20px;
                list-style: none;
                
                li {
                    padding-bottom: 15px;
                    margin-bottom: 20px;
                    border-bottom: #ababab solid 1px;
                    font-size: 0.7em;
                    &:first-of-type {
                            text-decoration: underline;
                        }
                    i {
                        margin-right: 10px;
                        color: #2477ca;
                    }
                    a {
                        color: #949494;
                        
                        transition: color 0.5s ease;
                        
                        &:hover {
                            color: #666666;
                        }
                    }
                }
            }
            }
        }
        .menu-footer {
            padding: 15px;
            font-size: 0.55em;
        }
    }
  }
  .nav-active {
        left: 0px;
    }

  </style>
  