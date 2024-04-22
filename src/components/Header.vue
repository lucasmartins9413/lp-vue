  <template>
    <header>  
        <a href="#" class="banner">
            Economize! Ganhe 61% OFF no seu primeiro pedido e um tigela grátias
        </a>
        <div class="container">
            <div class="area">
              <div class="logo">
                <a href=""><img width="120" height="40" src="@/assets/images/logo.png" alt="Logo DogDev"></a>
              </div>
              <div class="menu-opener">
                <div class="hamburguer-icon">
                  <span></span>
                  <span></span>
                  <span></span>
                </div>
                <div class="close-icon">
                  <span></span>
                  <span></span>
                </div>
              </div>
            </div>
            <nav>
              <ul>
                <li><a href="">Produtos</a></li>
                <li><a href="">Acessórios</a></li>
                <li><a href="">Depoimentos</a></li>
                <li><a href="">Minha conta</a></li>
                <li><a href="" class="bold">Comece agora</a></li>
              </ul>
            </nav>
        </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header',
    props: {
      title: {
        type: String,
        required: true,
      }
    }
  }
  </script>
  
  <style scoped>

  header{
    position: sticky;
    inset: 0 0 auto 0;
    z-index: 10;
    box-shadow: 0 0 5px #ccc;
    background: var(--background);
  }

  header .banner{
    display:block;
    background-color: var(--thirdground);
    padding: 1rem 2rem;
    text-align: center;
    color: var(--primary);
    text-decoration: none;
    font-weight: 600;
  }

  header .banner:hover{
    opacity: 0.8;
  }


  header .logo{
    height: auto;
  }

  header .area{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 2rem;
  }

  header .menu-opener{
    width: 2.5rem;
    height: 2.5rem;
    cursor: pointer;
  }

  header .hamburguer-icon{
    display: flex;
    flex-direction: column;
    height: 100%;
    justify-content: space-between;
  }

  header .hamburguer-icon span{
    display: block;
    width: 100%;
    height: 0.2rem;
    background-color: var(--secondary);
  }

  header .close-icon{
    display: none;
    flex-direction: column;
    height: 100%;
    justify-content: center;
    position: relative;
  }

  header .close-icon span{
    position: absolute;
    display: block;
    width: 100%;
    height: 0.2rem;
    background-color: var(--secondary);
  }

  header .close-icon span:first-child{
      transform: rotate(45deg);
  }

  header .close-icon span:last-child{
      transform: rotate(-45deg);
  }


  </style>