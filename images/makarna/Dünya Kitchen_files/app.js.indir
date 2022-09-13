const product_1 = new Product("images/hamburger/hamburger.png","Hamburger","3.75$","Patetes Kızartması ve Hamburgerin Enfes Buluşması",1)
const product_2 = new Product("images/hamburger/double-cheese-burger.png", "Double Cheese Burger", "3.25$", "Odun Ateşinde Double Cheese Burger",1);
const product_3 = new Product("images/hamburger/grilled-chicken-burger.png", "Köfte - Tavuk Hamburger", "2.95$", "Köfte Ve Tavuğun En Güzel Buluşması",1)
const product_4 = new Product("images/makarna/spagetti.jpg", "Spagetti Makarna", "2.45$", "İtalyan Usulü Spagetti Makarna", 3)
const product_5 = new Product("images/makarna/salcali-kelebek-makarna.webp", "Kelebek Makarna", "3.25$", "Salça İle Buluşmuş Harika Lezzet", 3)
const product_6 = new Product("images/makarna/makarna.png", "Makarna Etli", "3.35$", "Et İle Buluşmuş Harika Lezzet", 3)
const product_7 = new Product("images/makarna/kremali-makarna-.jpg", "Kremali Makarna", "3.75$", "Krema İle Buluşmuş Harika Lezzet", 3)
const product_8 = new Product("images/makarna/kremalı-makarna.jpg", "Kremali Mantarlı Makarna", "3.55$", "Krema ve Mantar İle Buluşmuş Harika Lezzet", 3)
const product_9 = new Product("images/pizza/biber-pissa.png", "Kırmızı Biberli Pizza", "3.55$", "Kalın Kenarlı Kırmızı Biberli Pizza", 0)
const product_10 = new Product("images/pizza/pizza.png", "Karışık Pizza", "3.95$", "İnce Kenarlı Kırmızı Karışık Pizza", 0)
const product_11 = new Product("images/pizza/sucuklu-pissa.png", "Sucuklu Pizza", "3.65$", "Harika Lezzetli Sucuklu Pizza", 0)
const product_12 = new Product("images/pizza/tomato-slices-pepperoni.png", "Kaşarlı Domatesli Bol Karışık Pizza", "4.25$", "Bol Peynilirli Domatesli Karışık  Pizza", 0)

const productList = [
    product_1,product_2,product_3,product_4,product_5,product_6,product_7,product_8,product_9,product_10,product_11,product_12
];
const product = document.querySelector("#product");
const productFull= () =>{
    product.innerHTML = "";
    productList.forEach(element => {
        product.innerHTML += `
                    <div class="col">
                                <div class="card-product">
                                        <div class="image">
                                            <div class="card-image">
                                                <img src="${element.image}" alt="" class="card-img">
                                            </div>
                                        </div>
                                        <div class="text">
                                            <h3>${element.title}</h3>
                                            <p class="d-none d-sm-block active">${element.text}" </p>
                                            <h4>${element.price}"</h4>
                                        </div>
                                </div>
                                </div>
                    `
    })
}
const productFilter = (filtre) => {
    product.innerHTML = "";
    productList.forEach(element => {
        if(element.id == filtre)
        product.innerHTML += `
                    <div class="col">
                                <div class="card-product">
                                        <div class="image">
                                            <div class="card-image">
                                                <img src="${element.image}" alt="" class="card-img">
                                            </div>
                                        </div>
                                        <div class="text">
                                            <h3>${element.title}</h3>
                                            <p class="d-none d-sm-block active">${element.text}" </p>
                                            <h4>${element.price}"</h4>
                                        </div>
                                </div>
                                </div>
                    `
    })
}
productFull();
const selection1 = document.querySelector(".swiper-wrapper")
selection1.addEventListener("click",filter,false)

function filter(element){
    console.log(element.target.id)
    if(element.target.id == 2){
      productFull();
    }
    else if(element.target.id == 0){
       productFilter(0)
    }
    else if (element.target.id == 1) {
        productFilter(1)
    }

    else if (element.target.id == 3) {
        productFilter(3)
    }


    
}