# biosal
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>คำนวณ BIOSAL 300</title>
</head>

<body style="font-family:sans-serif; text-align:center; padding:20px;">

<h1>ยาฆ่าเชื้อ BIOSAL 300</h1>
<h3>อัตรา 1 ml ต่อน้ำ 400 ml</h3>

<br>

<button style="font-size:26px; padding:25px; width:100%;"
onclick="calc(20)">
ถัง 20 ลิตร
</button>

<br><br>

<button style="font-size:26px; padding:25px; width:100%;"
onclick="calc(200)">
ถัง 200 ลิตร
</button>

<br><br>

<button style="font-size:26px; padding:25px; width:100%;"
onclick="calc(1000)">
ถัง 1000 ลิตร
</button>

<br><br><hr><br>

<h1 id="result">กดเลือกขนาดถัง</h1>

<script>
function calc(liter){
  let chemical = (liter * 1000) / 400;
  document.getElementById("result").innerText =
    "ต้องใส่ยา " + chemical + " ml";
}
</script>

</body>
</html>
