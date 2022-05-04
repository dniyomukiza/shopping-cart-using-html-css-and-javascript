# shopping-cart-using-html-css-and-javascript


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shopping Cart</title>
    <!-- CSS only -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-eOJMYsd53ii+scO/bJGFsiCZc+5NDVN2yr8+0RDqr0Ql0h+rP48ckxlpbzKgwra6" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/uikit@3.6.19/dist/css/uikit.min.css" />
    <script src="https://kit.fontawesome.com/33e495fb35.js" crossorigin="anonymous"></script>
    <link rel = 'stylesheet' href = 'shopping.css'>
    <script src="shopping.js" defer></script>
</head>
<body>
    <nav class="navbar navbar-dark bg-dark" style = 'height: 100px'>
        <div class="container-fluid">
          <h2  style = 'color: white'>Shoprite Store</h2>
          <i class="fas fa-cart-arrow-down"></i>
        </div>
      </nav>

      <div class = 'container'>
          <div class = 'row'>
              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/gold.png" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">Gold chair</h3>
                      <h4 class="card-text">$50</h4>
                      <a class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>

              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/infl1.png" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">Inflatable</h3>
                      <h4 class="card-text">$200</h4>
                      <a  class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>

              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/paspeaker.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">P.A speaker</h3>
                      <h4 class="card-text">$50</h4>
                      <a class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>


              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/Champagne.png" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">Champagne chair</h3>
                      <h4 class="card-text">$100</h4>
                      <a class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>

              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/jbl.jpg" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">JBL speaker</h3>
                      <h4 class="card-text">$30</h4>
                      <a class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>

              <div class = 'col-md-4 col-lg-4'>
                <div class="card" style="width: 18rem;">
                    <img src="images/infl2.png" class="card-img-top" alt="...">
                    <div class="card-body">
                      <h3 class="card-title">Adrenaline inflatable</h3>
                      <h4 class="card-text">$100</h4>
                      <a class="btn btn-primary">Add to Cart</a>
                    </div>
                  </div>
              </div>

          </div>
      </div>

      <div class="uk-overflow-auto container" style = 'width: 70%'>
        <table class="uk-table uk-table-hover uk-table-middle uk-table-divider">
            <thead>
                <tr>
                    <th class="uk-table-shrink"></th>
                    <th class="uk-table-small sty"><h3>ITEM</h3></th>
                    <th class="uk-table-small"></th>
                    <th class="uk-width-small sty"><h3>PRICE</h3></th>
                    <th class="uk-table-shrink uk-text-small sty"><h3>QUANTITY</h3></th>
                    <th class="uk-table-shrink uk-text-small sty"><h3>TOTAL</h3></th>

                </tr>
            </thead>
            
            <tr>
              <td><input class="uk-checkbox" type="checkbox"></td>
              <td><img class="uk-preserve-width uk-border-circle"  width="40" alt=""></td>
              <td class="uk-table-link">
                  <h3 class = "item-name"><strong>Grand-Total</strong></h3>
              </td>
              <td class="uk-text-truncate"><h3></h3></td>
              <td class="uk-text-truncate"><h3></h3></td>
              <td class="uk-text-truncate grand-total"><h3><strong>$0</strong></h3></td>

          </tr>
          
        </table>
    </div>
</body>
</html>

=============================CSS=====================================================================================================================================
.container{
    margin: auto;
    margin-top: 20px;
    border: 3px solid whitesmoke; 
    background-color:blanchedalmond;
}
.col-md-, .col-lg-4{
    margin-bottom: 20px;
    
}
.sty{
    font-size: 18px !important;
    color: black !important;
}
.num{
    width: 80px;
    height: 30px;
    border: 3px solid black;
    border-radius: 5px;
    font-size: 18px;
    padding: 5px;
}
.uk-border-circle{
    width: 100px !important;
    height: 100px !important;
}
.fa-cart-arrow-down{
    color: white;
    font-size: 50px;
    cursor: pointer;
    padding-left: 20px;
}

.card-img-top{
    height: 150px;
     width:150px;
    }
    
     =================================================================JAVASCRIPT===========================================================
     let add_to_cart_btns = document.getElementsByClassName('btn-primary');
let main_container = document.getElementsByTagName('tbody')[0];
let quantity_fields = document.getElementsByClassName('num')
let removeBtns = document.getElementsByClassName('uk-button-danger');

for(let i = 0; i < add_to_cart_btns.length; i++) {
    add_to_cart_btns[i].addEventListener('click', addToCart)
    }
function addToCart(event){
    let btn = event.target;
    let btn_parent = btn.parentElement;
    let btn_grandparent = btn.parentElement.parentElement;
    let itemName = btn_parent.children[0].innerText;
    let itemPrice = btn_parent.children[1].innerText;
    let itemImage = btn_grandparent.children[0].src;

    let itemContainer = document.createElement('tr')
    itemContainer.innerHTML = `<td><input class="uk-checkbox" type="checkbox"></td>
    <td><img class="uk-preserve-width uk-border-circle" src="${itemImage}" width="40" alt=""></td>
    <td class="uk-table-link">
        <h3 class = "item-name">${itemName}</h3>
    </td>
    <td class="uk-text-truncate item-price"><h3>${itemPrice}</h3></td>
    <td><input type = 'number' class = 'num' value = '1'></td>
    <td class="uk-text-truncate total-price"><h3>${itemPrice}</h3></td>
    <td><button class="uk-button uk-button-danger" type="button">Remove</button></td>`
   main_container.append(itemContainer);

   //loop throug quantities of items
for(let i = 0; i < quantity_fields.length; i++) {
    quantity_fields[i].addEventListener('change', updateTotal)
    }
    //remove option appears after adding to cart,thus for has to be here
for(let i = 0; i < removeBtns.length; i++) {
        removeBtns[i].addEventListener('click', removeItem)
        }
    grandTotal(); //whenever we add cart,add price to grand total
    function updateTotal(event){
        number_of_items = event.target;
        number_of_items_parent = number_of_items.parentElement.parentElement;
        price_field = number_of_items_parent.getElementsByClassName('item-price')[0]; 
        total_field = number_of_items_parent.getElementsByClassName('total-price')[0];
        price_field_content = price_field.children[0].innerText.replace('$', '');
        total_field.children[0].innerText = '$' + number_of_items.value * price_field_content;
     //customer has to order at least one item

     if(isNaN(number_of_items.value) || number_of_items.value <= 0) {
         number_of_items.value = 1;
     }
     grandTotal();//increase number should update grandtotal
    }

   function grandTotal(event){
       let total = 0;
       let grand_total = document.getElementsByClassName('grand-total')[0];
       let total_price = document.getElementsByClassName('total-price');
       for(let i = 0; i < total_price.length; i++) {
       total_price_content = Number(total_price[i].innerText.replace('$', ''));
       total += total_price_content;
    }
    grand_total.children[0].innerText = '$' +total;//put cost into grand total
    grand_total.children[0].style.fontWeight = 'bold'
}
function removeItem(event){
    remove_btn = event.target//each rmv button we target,click on
    remove_btn_grandparent = remove_btn.parentElement.parentElement
    remove_btn_grandparent.remove();
    grandTotal();//whenever we remove item, grand total should lways be called to update
}   
} 
