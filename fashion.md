var man=[
    {
    id:1,
    name:"Quần tây",
    code:"TC143NA",
    price:"300.000",
    image:"https://product.hstatic.net/1000392326/product/msc5003_-_768k__mqd5013_-_738k__1__7c20449c6b2745c987b8b57ffabb7503_master.jpg"
    },
    {
    id:2,
    name:"Áo sơ mi nam",
    code:"TC1342NA",
    price:"400.000",
    image:"https://product.hstatic.net/1000392326/product/msc3001_-_768k___mqd5008_-_738k_3__88b3f6687f3d4d43a0160d63f20d6ef6_master.jpg"
    },
    {
    id:3,
    name:"Áo khoác",
    code:"TC323",
    price:"500.000",
    image:"https://product.hstatic.net/1000360022/product/id-006085a_43f248de46d44fa587f0aa921e3df868_1024x1024.jpg"
    },
    {
    id:4,
    name:"Áo polo",
    code:"TC223",
    price:"250.000",
    image:"https://4men.com.vn/images/thumbs/2023/05/ao-polo-mat-chim-co-v-theu-wave-form-slimfit-po107-mau-xam-18013-slide-products-645b14111245f.jpg"
    }

]
var women=[
    {
    id:1,
    name:" áo vest công sở ",
    code:"TC143",
    price:"450.000",
    image:"https://product.hstatic.net/1000392326/product/bad13053_-_1168k_bai33009_-_398k_bjd13053_-_668k__9__975b52c180b24ea28d735c34c487b570_master.jpg"
    },
    {
    id:2,
    name:"Áo sơ mi nữ",
    code:"TC123",
    price:"300.000",
    image:"https://product.hstatic.net/1000392326/product/fas53617_-_798k_fqd51090_-_888k__1__f769ce34731c41f3be6ba618b0012308_master.jpg"
    },
    {
    id:3,
    name:"Chân váy",
    code:"TC323",
    price:"590.000",
    image:"https://product.hstatic.net/1000392326/product/fas53588_-_868k_bjd72884_-_1188k___1__6928e4058f8848cd84dfb2d09d61491e_master.jpg"
    },
    {
    id:4,
    name:"Áo thun",
    code:"TC223",
    price:"780.000",
    image:"https://product.hstatic.net/1000392326/product/fvo042_-_2768k_fol341_-_668k_fqn7342_-_868k___1__3fc83880fa764b90aa887a5bf3db8495_master.jpg"
    }
]
function listProducts(){
    for(let i=0; i<= man.length-1;i++){
        var demo = '<div class="col-3">';
        demo+= '<div class="card" style="width: 18rem; ">';
        demo+= '<img src="'+man[i].image+'" class="card-img-top" style="height:400px; ">';
        demo += '<div class="card-body">';
        demo += '<h5 class="card-title">'+man[i].name+'</h5>';
        demo += '<p class="card-text">'+man[i].price+'</p>';
        demo += '<a href="#" class="btn btn-primary" onclick="oder()">Đặt mua</a>';
        demo += '</div>';
        demo += '</div>';
        demo += '</div>';
        console.log(demo);
        document.getElementById("men").innerHTML+= demo;


    }
    for(let i=0; i<= women.length-1;i++){
        var demo = '<div class="col-3">';
        demo+= '<div class="card" style="width: 18rem; ">';
        demo+= '<img src="'+women[i].image+'" class="card-img-top" style="height:400px; ">';
        demo += '<div class="card-body">';
        demo += '<div class="card-title">'+women[i].name + '</h5>';
        demo += '<p class="card-text">'+women[i].price+'</p>';
        demo += '<a href="#" class="btn btn-primary" onclick="oder()">Đặt mua</a>';
        demo += '</div>';
        demo += '</div>';
        demo += '</div>';
        console.log(demo);
        document.getElementById("women").innerHTML+= demo;


    }

}
