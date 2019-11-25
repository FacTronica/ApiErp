# CURL Enviar Datos Json

<br>$data = json_decode($json); 
<br>$url = "http://www.factronica.cl/api/ventas_documentos_boletas/index.php";
<br>$curl = curl_init($url);
<br>curl_setopt($curl, CURLOPT_HEADER, false);
<br>curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);
<br>curl_setopt($curl, CURLOPT_HTTPHEADER,array("Content-type: application/json"));
<br>curl_setopt($curl, CURLOPT_POST, true);
<br>curl_setopt($curl, CURLOPT_POSTFIELDS, $json);
<br>$json_response = curl_exec($curl);
<br>$status = curl_getinfo($curl, CURLINFO_HTTP_CODE);
<br>curl_close($curl);
<br>echo "FolioBoleta=".$json_response; 
