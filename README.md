<!DOCTYPE html>
<html>
<head>
    <title>Aplikasi Konversi Mata Uang</title>
    <link rel="stylesheet" href="assets/css/bootstrap.min.css">
    <link rel="stylesheet" type="text/css" href="bootstrap.css">
	<style type="text/css">
		#dt{
			width: 5%;
			border: 0;
		}
		#border{
			border: 0;
		}
	</style>
</head>
    </style>
</head>
FadhilRaz: <head>
    <meta charset= "utf-8">
    <meta name= "viewport" content= "width= device-width, intial-scale= 1.0">
    <style media= "screen">
        body{
            background:linear-gradient(#000428, #004e92);
            color: white;
            font-style: oblique;
        }
        @media only screen and (min-width:600px){
            body{
                background: linear-gradient(#000428, #004e92);
                color: white;
                font-style: oblique;
            }
        }
        @media only screen and (min-width:600px){
            body{
                background:linear-gradient(#000428, #004e92);
                color: white;
                font-style:oblique;
            }
        }</Style>
<body style="background-color: linear-gradient(#000428 #004e92); background-position: center; background-size: 100% ">
<script>
	function convert() {

		var nilai = document.getElementById("nilai").value;
		var uang1 = document.getElementById("matauang1");
		var uang1value = uang1.options[uang1.selectedIndex].value;
		var uang1text = uang1.options[uang1.selectedIndex].text;

		var uang2 = document.getElementById("matauang2");
		var uang2value = uang2.options[uang2.selectedIndex].value;
		var uang2text = uang2.options[uang2.selectedIndex].text;

		var bantu = 1;
		var bantu1 = (bantu / uang1value);
		var bantu2 = bantu1*uang2value;
		var bantu3 = bantu2*nilai;

		document.getElementById("hasil").value = bantu3;
	}
</script>
<!-- <center><img src="bitmap.png" style="width: 200px; height: 200px"></center>
<br> -->

 <center>
 	<h1 style="color: #BA8B02; margin-top: 10%">Aplikasi Konversi Mata Uang</h1><br><br>
		
		<table border="5" style="width: 60%; height: 50%; border-color: white; color: white" cellpadding="10" >
			<tr>
				<td id="border">
					Mata Uang Asal
				</td>
				<td id="dt">
					
				</td>
				<td id="border">
					Mata Uang Tujuan
				</td>
			</tr>
			<tr>
				<td id="border">
					<select id="matauang1" class="form-control form-control-lg">
					<option selected="selected" value="1" >IDR</option>
					<option value="0.000054">Poundsterling</option><option value="0.000072">USD</option>
					</select>
				</td>
				<td id="border">
					
				</td>
				<td id="border">
					<select id="matauang2" class="form-control form-control-lg"> 
					<option selected="selected" value="1">IDR</option>
					<option value="0.000054">Poundsterling</option>
					<option value="0.000072">USD</option>
					</select> 
				</td>
			</tr>
			<tr>
				<td id="border">
					 <input id="nilai" type="text"  class="form-control" placeholder="Masukkan nilai">
				</td>
				<td id="dt">
					
				</td>
				<td id="border">
					<input type="text" id="hasil" name="" readonly=""style="background-color: rgba(236,236,236,255);" width="100%" height="100%" class="form-control" placeholder="Hasil">
				</td>
			</tr>
			<tr>
				<td colspan="3" id="border">
					<button type="submit" class="btn btn-success" onclick="convert();" style="height: 100%; width: 10%">Hitung</button>
				</td>
			</tr>
		</table>
</center>
</body>
</html>
</body>
</html>
