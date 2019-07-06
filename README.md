<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <?php 
        $a = "";
        $b = "";
        if($_SERVER["REQUEST_METHOD"] == "POST"){
            $a = $_POST["bakcolor"];
            $b = $_POST["color"];
        }
    ?>
    <div class="box1" id="frm">
        <div class="box11">Định màu chữ và màu nền</div>
        <div class="box12">
            <form method="POST" action="form.html">
                <span>Nội dung</span>
                <input type="text" value="Thay đổi"> <br>
                <span>Màu nền</span>
                <input type="text" name="bakcolor"> <br>
                <span>Màu chữ</span>
                <input type="text" name="color">
                <br>
                <input type="submit" id="nhap" onclick="chay();" value="Xem kết quả" class="fix">
                <h5 id="h5m">
                    name
                </h5>
            </form>
        </div>
    </div>
    <div class="box1">
        <div class="box11">Diện tích hình chữ nhật</div>
        <div class="box12">
            <form method="POST" action="form.html">
                <span>Chiều dài</span>
                <input type="text"> <br>
                <span>Chiều rộng</span>
                <input type="text" id="bakcolor"> <br>
                <span>Diện tích</span>
                <input type="text" id="color">
                <br>
                <input type="submit" id="nhap" value="Xem kết quả" class="fix">

            </form>
        </div>
    </div>
    <div class="box1">
        <div class="box11">Diện tích và chu vi hình tròn</div>
        <div class="box12">
            <form method="POST" action="form.html">
                <span>Bán kính</span>
                <input type="text"> <br>
                <span>Diện tích</span>
                <input type="text" id="bakcolor"> <br>
                <span>Chu vi</span>
                <input type="text" id="color">
                <br>
                <input type="submit" id="nhap" value="Xem kết quả" class="fix">

            </form>
        </div>
    </div>

    <div class="box1">
        <div class="box11">Thanh toán tiền điện</div>
        <div class="box12">
            <form method="POST" action="form.html">
                <span>Tên chủ hộ</span>
                <input type="text"> <br>
                <span>Chi số cũ</span>
                <input type="text" id="bakcolor">
                <p>(kW)</p>
                <span>Chi số mới</span>
                <input type="text" id="color">
                <p>(kW)</p>
                <span>Đơn giá</span>
                <input type="text" id="color" value="2000">
                <p>(VNĐ)</p>
                <span>Thành tiền</span>
                <input type="text" id="color">
                <p>(VNĐ)</p>
                <br>
                <input type="submit" id="nhap" value="Xem kết quả" class="fix">

            </form>
        </div>
    </div>
    <div class="box1">
        <div class="box11">Cạnh huyền tam giác vuông</div>
        <div class="box12">
            <form method="POST" action="form.html">
                <span>Canh A</span>
                <input type="text"> <br>
                <span>Canh B</span>
                <input type="text" id="bakcolor"> <br>
                <span>Canh huyền</span>
                <input type="text" id="color">
                <br>
                <input type="submit" id="nhap" value="Xem kết quả" class="fix">

            </form>
        </div>
    </div>
    <script type="text/javascript">
	function submitForm(){
		//tac dong vao the html co id=frm, thuc hien submit form
		document.getElementById("frm").submit();
	}
</script>
</body>

</html>
