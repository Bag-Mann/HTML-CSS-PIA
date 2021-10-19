# HTML-CSS-PIA

*/ FORMULARIO Y LOGOS DE USUARIO Y CARRITO*/
HTML
  <link rel="stylesheet" href="">
          <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/all.min.css">
          <div class="main-header__container">
              <i class="fas fa-user"></i>
              <a href="main-header__btn">Mi Carrito<i class="fas fa-shopping-cart"></i></a>
              <input type="search" class="main-header__input" placeholder="Buscar productos"><i class="fas fa-search"></i>
          </div>
CSS
  .main-header__container{
      display: flex;
      justify-content:end;
      align-items: center;
  }
  .main-header__btn{
      display: block;
      padding: 10px 25px;
      color: #454546;
      border: 1px solid #454546;
      text-decoration: none;
  }
  
/*  PRODUCTOS */
HTML
<main class="main">
            <h3 class="main-title">Nuevos productos para ti</h3>
            <section class="container-products">
            <div class="product">
                <img width="300" src="https://cdn1.coppel.com/images/catalog/pr/5128132-1.jpg" alt="" class="product__img">
                <div class="product__description">
                    <h3 class="product__title"> Gorra Superman</h3>
                    <span class="product__price">$50.50</span>
            </div>
                <i class="product__icon fas fa-shopping-basket"></i>
            </div>
            <div class="product">
                <img width="200" src="https://cdn1.coppel.com/images/catalog/pr/2060022-1.jpg" alt="" class="product__img">
                <div class="product__description">
                    <h3 class="product__title"> Gorra Iron Man</h3>
                    <span class="product__price">$30.50</span>
            </div>
                <i class="product__icon fas fa-shopping-basket"></i>
            </div>
            </section>
        </main>
        
CSS
  .container-products{
      display: grid;
      grid-template-columns:repeat(2,1fr);
      grid-gap: 10px;
  }
  .product{
      border: 2px solid #cccc;
      padding: 20px;
      text-align: center;
      position: relative;
  }
  .product:before {
      content: "NUEVO";
      background: #FF4E00;
      padding: 10px;
      position: absolute;
      top: 25px;
      right: 10px;
      transform: rotate(-90deg);
      color: white;
  }
  .product__title{
      text-align: center;
  }
  .product__price{
      color: #FF4E00;
      font-weight: bold;
  }
  .product__icon{
      display: block;
      margin: 10px 0;
  }
  .product__img{
      width: 100%;
    height: 120px;
    object-fit: cover;
}
