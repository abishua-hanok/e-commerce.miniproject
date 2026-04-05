const products = [
  { id: 1, name: "Product 1", price: 100 },
  { id: 2, name: "Product 2", price: 200 },
  { id: 3, name: "Product 3", price: 300 }
];

let cart = [];

function displayProducts() {
  const container = document.getElementById("products");
  container.innerHTML = "";
  products.forEach(p => {
    container.innerHTML += `
      <div class="card">
        <h3>${p.name}</h3>
        <p>₹${p.price}</p>
        <button onclick="addToCart(${p.id})">Add to Cart</button>
      </div>
    `;
  });
}

function addToCart(id) {
  const item = products.find(p => p.id === id);
  cart.push(item);
  updateCart();
}

function updateCart() {
  document.getElementById("cart-count").innerText = cart.length;
  const list = document.getElementById("cart-items");
  list.innerHTML = "";
  cart.forEach(item => {
    list.innerHTML += `<li>${item.name} - ₹${item.price}</li>`;
  });
}

function viewCart() {
  document.getElementById("cart").classList.remove("hidden");
}

function closeCart() {
  document.getElementById("cart").classList.add("hidden");
}

displayProducts();
