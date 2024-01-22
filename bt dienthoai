<!DOCTYPE html>
<html>
<head>
    <title>Oak Lump</title>
    <style>
        #cart {
            list-style-type: none;
            padding: 0;
        }
        .cart-item {
            border: 1px solid #ddd;
            margin-bottom: 10px;
            padding: 10px;
        }
        .cart-item img {
            width: 446px;
            height: auto;
            margin-right: 10px;
        }   
        button {
            padding: 10px 20px;
            border: none;
            border-radius: 3px;
            cursor: pointer;
        }

        button[type="button"] {
            background-color: #0074D9; /* Màu xanh dương cho nút "Thêm sản phẩm" */
            color: white;
        }

        button[type="button1"] {
            background-color: #4CAF50; /* Màu xanh lá cho nút "Đặt mua" */
            color: white;
        }
    </style>
</head>
<body>
    <form name="SunShine">
        <p>
            <label>
                Product Name:
                <input type="text" name="pro" id="pro"/>
            </label>
            <label>
                Product Picture:
                <input type="file" name="image" id="image" accept="image/*"/>
            </label>
            <label>
                Product price:
                <input type="number" name="pri" id="pri"/>
            </label>
        </p>
    </form>
    <button type="button" onclick="add()">Thêm sản phẩm</button>
    <div>
        <h2>Điện thoại nổi bật nhất</h2>
        <ul id="cart"></ul>
    </div>
    <script type="text/javascript">
        function add(){
            var image = document.getElementById("image").files[0];
            var pro = document.getElementById("pro").value;
            var pri = document.getElementById("pri").value;
            var reader = new FileReader();
            reader.onload = function(e) {
                var imgSrc = e.target.result;
                var cartItem = document.createElement('li');
                cartItem.className = 'cart-item';
                cartItem.innerHTML = `
                    <img src='${imgSrc}' alt='Product Image' />
                    <div>
                        <p><strong>Product : ${pro}</strong></p>
                        <p>Price: ${pri}</p>
                    </div>
                `;
                document.getElementById("cart").appendChild(cartItem);
            };
            reader.readAsDataURL(image);
        } 
    </script>
    <button type="button1" onclick="datmua()">Đặt mua</button>
</body>
</html>
