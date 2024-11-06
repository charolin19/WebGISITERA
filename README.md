# WebGISITERA
GEDUNG ITERA
<html>
<head>
   <title>Belajar WebGIS</title>
   <!-- LEAFLET CSS -->
   <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
   <style>
      #map{
          width: 100%;
          height: 100vh;
      }
  </style>
</head> 
   <body>
     <div id="map"></div>
   </body>
</html>
   <!-- LEAFLET JAVASCRIPT -->
   <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
   <script>
   <!-- LOKASI KAJIAN -->
   var map = L.map('map').setView([-5.367016, 105.317890], 15);
      <!-- BASEMAP OPENSTREETMAP -->
   var osm = L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
       attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
       });
       osm.addTo(map);
       <!-- BASEMAP ESRI -->
   var Esri_WorldImagery = L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
       attribution: 'Tiles &copy; Esri &mdash; Source: Esri, i-cubed, USDA, USGS, AEX, GeoEye, Getmapping, Aerogrid, IGN, IGP, UPR-EGP, and the GIS User Community'
       });
   Esri_WorldImagery.addTo(map);
       <!-- POSISI GEDUNG F -->
       //L.marker([ -5.361372, 105.313723]).addTo(map);
       <!-- POSISI GEDUNG E -->
       //L.marker([  -5.359985, 105.315545] ).addTo(map);
       <!-- POSISI EMBUNG A -->
       //L.marker([  -5.357727, 105.312782]).addTo(map);
       <!-- POSISI GEDUNG GKU 1 -->
       //L.marker([-5.360920, 105.310511]).addTo(map);
       <!-- POSISI GEDUNG LABTEK OZT -->
       //L.marker([-5.362487,105.310674]).addTo(map);
       <!-- POSISI GEDUNG  A -->
       //L.marker([  -5.357948,105.314397]).addTo(map);
       <!-- POSISI GEDUNG  B -->
       //L.marker([  -5.357924,105.315331]).addTo(map);
       <!-- POSISI GEDUNG  C dan D -->
       //L.marker([  -5.358407,105.313694]).addTo(map);
       <!-- POSISI GEDUNG  Laboratorium 1 -->
       //L.marker([  -5.360321,105.310236]).addTo(map);
       <!-- POSISI GEDUNG  Laboratorium 2 -->
       //L.marker([  -5.361516,105.310534]).addTo(map);
       <!-- POSISI GEDUNG  Laboratorium 3 -->
       //L.marker([  -5.360294,105.309135]).addTo(map);
       <!-- POSISI  Embung B -->
       //L.marker([  -5.359044,105.308088]).addTo(map);
       <!-- POSISI  Embung C -->
       //L.marker([  -5.359404,105.313704]).addTo(map);
       <!-- POSISI  Embung D -->
       //L.marker([  -5.360221,105.320753]).addTo(map);
       <!-- POSISI  Embung E -->
       //L.marker([  -5.365216,105.316825]).addTo(map);
       <!-- POSISI  Embung SUMATERA -->
       //L.marker([  -5.370186,105.310329]).addTo(map);
       <!-- POSISI  LABIRIN -->
       //L.marker([   -5.369667,105.312161]).addTo(map);
       <!-- POSISI GEDUNG  Kantin BKL -->
       //L.marker([  -5.357598,105.316519]).addTo(map);
       <!-- POSISI GEDUNG  Kantin RK -->
       //L.marker([  -5.359432,105.312622]).addTo(map);
       <!-- POSISI GEDUNG  RIMA -->
       //L.marker([  -5.358613,105.321090]).addTo(map);
       <!-- POSISI GEDUNG  Masjid Raya At Tanwir -->
       //L.marker([  -5.356767,105.318819]).addTo(map);
       <!-- POSISI GEDUNG  Masjid Baitul Ilmi  -->
       //L.marker([  -5.359054,105.312624]).addTo(map);
       <!-- POSISI GEDUNG  Asrama TB1 -->
       //L.marker([  -5.358414,105.317456]).addTo(map);
       <!-- POSISI GEDUNG  Asrama TB2 -->
       //L.marker([  -5.358449,105.319444]).addTo(map);
       <!-- POSISI GEDUNG  Asrama TB3 -->
       //L.marker([  -5.359123,105.319108]).addTo(map);
       <!-- POSISI GEDUNG  Asrama TB4 -->
       //L.marker([  -5.359131,105.317503]).addTo(map);
       <!-- POSISI GEDUNG  Asrama TB5 -->
       //L.marker([  -5.358468,105.318470]).addTo(map);
       <!-- POSISI GEDUNG  GSG -->
       //L.marker([  -5.362422,105.318954]).addTo(map);
       <!-- POSISI GEDUNG  Poliklinik ITERA -->
       //L.marker([  -5.357728,105.315966]).addTo(map);
       <!-- POSISI GEDUNG  ATM ITERA -->
       //L.marker([  -5.357590,105.315092]).addTo(map);
       <!-- POSISI GEDUNG  GALERI1 -->
       //L.marker([  -5.357906,105.315573]).addTo(map);
       <!-- POSISI PLTS -->
       //L.marker([   -5.360436,105.311861]).addTo(map);
      <!-- BUNDARAN YANG SERING SAYA LANGGAR ATURAN SAAT BERLALU LINTAS DI ITERA -->
      var bundaran = L.circle([ -5.363156, 105.312634], {
       color: 'red',
       fillColor: '#f03',
       fillOpacity: 0.5,
       radius: 20
       }).addTo(map);
      <!-- BUNDARAN INI JUGA SERING SAYA LANGGAR SETELAH SELESAI KULIAH DI GKU 2 -->
      var bundaran = L.circle([-5.360813, 105.314847], {
       color: 'green',
       fillColor: '#f03',
       fillOpacity: 0.5,
       radius: 35
       }).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG F -->
      var polygon = L.polygon([
       [-5.359799, 105.315831],
       [-5.359957, 105.315831],
       [-5.359957, 105.315571],
       [-5.360474, 105.315571],
       [-5.360474, 105.315401],
       [-5.359635, 105.315401],
       [-5.359635, 105.315571],
       [-5.359799, 105.315571]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG GKU1 -->
      var polygon = L.polygon([
       [-5.360815, 105.311007],
       [-5.361035, 105.311007],
       [-5.361051, 105.309973],
       [-5.360821, 105.309968]
       ]).addTo(map);
      <!-- POLIGON PLTS ITERA -->
      var polygon = L.polygon([
       [-5.360194, 105.311469],
       [-5.360869, 105.311469],
       [-5.360864, 105.312158],
       [-5.360724, 105.312153],
   	 [-5.360730, 105.312374],
       [-5.360553, 105.312368],
       [-5.360537, 105.312594],
	    [-5.360392, 105.312594],
       [-5.360387, 105.312826],
       [-5.360156, 105.312831]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG A -->
      var polygon = L.polygon([
       [-5.357717, 105.314304],
       [-5.357714, 105.314492],
       [-5.358094, 105.314497],
       [-5.358091, 105.314292]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG B -->
      var polygon = L.polygon([
       [-5.357714, 105.315242],
       [-5.357716, 105.315414],
       [-5.358076, 105.315423],
       [-5.358076, 105.315239]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  C dan D -->
      var polygon = L.polygon([
       [-5.358384, 105.313266],
       [-5.358377, 105.313447],
       [-5.358344, 105.313443],
       [-5.358359, 105.314091],
       [-5.358496, 105.313950],
       [-5.358494, 105.313567],
       [-5.358926, 105.313571],
       [-5.359111, 105.313376],
       [-5.358533, 105.313389],
       [-5.358536, 105.313267]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG E -->
      var polygon = L.polygon([
       [-5.359799, 105.315831],
       [-5.359957, 105.315831],
       [-5.359957, 105.315571],
       [-5.360474, 105.315571],
       [-5.360474, 105.315401],
       [-5.359635, 105.315401],
       [-5.359635, 105.315571],
       [-5.359799, 105.315571]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  Labaoratorium 1 -->
      var polygon = L.polygon([
       [-5.360213, 105.309928],
       [-5.360211, 105.310431],
       [-5.360381, 105.310439],
       [-5.360381, 105.310374],
       [-5.360447, 105.310364],
       [-5.360448, 105.309918]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG Laboratorium 2 -->
      var polygon = L.polygon([
       [-5.361431, 105.309937],
       [-5.361434, 105.310895],
       [-5.361611, 105.310904],
       [-5.361618, 105.309940]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG Laboratorium 3 -->
      var polygon = L.polygon([
       [-5.360165, 105.308750],
       [-5.360175, 105.309413],
       [-5.360437, 105.309415],
       [-5.360438, 105.308749]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG ASRAMA TB 1 -->
      var polygon = L.polygon([
       [-5.358361, 105.317140],
       [-5.358360, 105.317644],
       [-5.358547, 105.317645],
       [-5.358546, 105.317142]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG ASRAMA TB 2 -->
      var polygon = L.polygon([
       [-5.358396, 105.319140],
       [-5.358396, 105.319630],
       [-5.358583, 105.319642],
       [-5.358583, 105.319137]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG ASRAMA TB 3 -->
      var polygon = L.polygon([
       [-5.359095, 105.318720],
       [-5.359095, 105.319304],
       [-5.359231, 105.319311],
       [-5.359231, 105.318728]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG ASRAMA TB 4 -->
      var polygon = L.polygon([
       [-5.359075, 105.317113],
       [-5.359076, 105.317709],
       [-5.359207, 105.317721],
       [-5.359197, 105.317112]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG SERBAGUNA -->
      var polygon = L.polygon([
       [-5.362242, 105.318794],
       [-5.362252, 105.319000],
       [-5.362655, 105.319029],
       [-5.362664, 105.318794]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  POLIKLINIK ITERA -->
      var polygon = L.polygon([
       [-5.357662, 105.315927],
       [ -5.357660, 105.315950],
       [ -5.357687, 105.315956],
       [ -5.357687, 105.316005],
       [ -5.357794, 105.316013],
       [ -5.357799, 105.315925]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG Kantin RK -->
      var polygon = L.polygon([
       [-5.359279, 105.312453],
       [-5.359273, 105.312826],
       [-5.359620, 105.312825],
       [-5.359616, 105.312449]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  Kantin BKL -->
      var polygon = L.polygon([
       [-5.357500, 105.316221],
       [-5.357499, 105.316342],
       [-5.357445, 105.316344],
       [-5.357451, 105.316677],
       [-5.357685, 105.316677],
       [-5.357700, 105.316364],
       [-5.357633, 105.316362],
       [-5.357635, 105.316233]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  Masjid At Tanwir -->
      var polygon = L.polygon([
       [-5.356596, 105.318729],
       [-5.356738, 105.318985],
       [-5.357011, 105.318841],
       [-5.356915, 105.318625],
       [-5.356870, 105.318651],
       [-5.356859, 105.318605]
       ]).addTo(map);
      <!-- POLIGON BANGUNAN  GEDUNG Baitul Ilmi -->
      var polygon = L.polygon([
       [-5.359117, 105.312468],
       [-5.359212, 105.312657],
       [-5.359015, 105.312742],
       [-5.358926, 105.312558]
       ]).addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG F-->
    var GDGF = L.marker([-5.361372, 105.313723]);
    var namagdgf = GDGF.bindPopup("Gedung F").openPopup()
    namagdgf.addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG E-->
    var GDGE = L.marker([-5.359985, 105.315545]);
    var namagdge = GDGE.bindPopup("Gedung E").openPopup()
    namagdge.addTo(map);
   <!-- MENAMPILKAN NAMA EMBUNG A-->
    var EBGA = L.marker([-5.357727, 105.312782]);
    var namaebga = EBGA.bindPopup("Embung A").openPopup()
    namaebga.addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG GKU 1 -->
    var GKU1 = L.marker([-5.360920, 105.310511]);
    var namagku1 = GKU1.bindPopup("Gedung GKU 1").openPopup()
    namagku1.addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG Laboratorium OZT -->
    var LaboratoriumOZT = L.marker([-5.362487,105.310674]);
    var namaLaboratoriumOZT = LaboratoriumOZT.bindPopup("Laboratorium OZT").openPopup()
    namaLaboratoriumOZT.addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG GKU 2 -->
    var GKU2 = L.marker([-5.360267,105.314202]);
    var namagku2 = GKU2.bindPopup("Gedung GKU 2").openPopup()
    namagku2.addTo(map);
    <!-- MENAMPILKAN NAMA GEDUNG A -->
    var A = L.marker([-5.357948,105.314397]);
    var namaA = A.bindPopup("Gedung A").openPopup()
    namaA.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG B -->
    var B = L.marker([-5.357924,105.315331]);
    var namaB = B.bindPopup("Gedung B").openPopup()
    namaB.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG C dan D -->
    var CdanD = L.marker([-5.358407,105.313694]);
    var namaCdanD = CdanD.bindPopup("Gedung C dan D").openPopup()
    namaCdanD.addTo(map);
   <!-- MENAMPILKAN NAMA GEDUNG Laboratorium 1 -->
    var Laboratorium1 = L.marker([-5.360321,105.310236]);
    var namaLaboratorium1 = Laboratorium1.bindPopup("Laboratorium 1").openPopup()
    namaLaboratorium1.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Laboratorium 2 -->
    var Laboratorium2 = L.marker([-5.361516,105.310534]);
    var namaLaboratorium2 = Laboratorium2.bindPopup("Laboratorium 2").openPopup()
    namaLaboratorium2.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Laboratorium 3 -->
    var Laboratorium3 = L.marker([-5.360294,105.309135]);
    var namaLaboratorium3 = Laboratorium3.bindPopup("Laboratorium 3").openPopup()
    namaLaboratorium3.addTo(map);
    <!-- MENAMPILKAN NAMA Embung B -->
    var EmbungB = L.marker([-5.359044,105.308088]);
    var namaEmbungB = EmbungB.bindPopup("Embung B").openPopup()
    namaEmbungB.addTo(map);
	<!-- MENAMPILKAN NAMA Embung C -->
    var EmbungC = L.marker([-5.359404,105.313704]);
    var namaEmbungC = EmbungC.bindPopup("Embung C").openPopup()
    namaEmbungC.addTo(map);
	<!-- MENAMPILKAN NAMA Embung D -->
    var EmbungD = L.marker([-5.360221,105.320753]);
    var namaEmbungD = EmbungD.bindPopup("Embung D").openPopup()
    namaEmbungD.addTo(map);
	<!-- MENAMPILKAN NAMA Embung E -->
    var EmbungE = L.marker([-5.365216,105.316825]);
    var namaEmbungE = EmbungE.bindPopup("Embung E").openPopup()
    namaEmbungE.addTo(map);
	<!-- MENAMPILKAN NAMA Embung SUMATERA -->
    var EmbungSumatera = L.marker([-5.370186,105.310329]);
    var namaEmbungSumatera = EmbungSumatera.bindPopup("Embung SUMATERA").openPopup()
    namaEmbungSumatera.addTo(map);	
	<!-- MENAMPILKAN NAMA LABIRIN -->
    var Labirin = L.marker([-5.369667,105.312161]);
    var namaLabirin = Labirin.bindPopup("LABIRIN").openPopup()
    namaLabirin.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Kantin BKL -->
    var KantinBKL = L.marker([-5.357598,105.316519]);
    var namaKantinBKL = KantinBKL.bindPopup("Kantin BKL").openPopup()
    namaKantinBKL.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Kantin RK -->
    var KantinRK = L.marker([-5.359432,105.312622]);
    var namaKantinRK = KantinRK.bindPopup("Kantin RK").openPopup()
    namaKantinRK.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG RIMA -->
    var RIMA = L.marker([-5.358613,105.321090]);
    var namaRIMA = RIMA.bindPopup("Rumah Ibadah Multi Agama").openPopup()
    namaRIMA.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Masjid Raya At Tanwir -->
    var MasjidRayaAtTanwir = L.marker([-5.356767,105.318819]);
    var namaMasjidRayaAtTanwir = MasjidRayaAtTanwir.bindPopup("Masjid Raya At-Tanwir").openPopup()
    namaMasjidRayaAtTanwir.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Masjid Baitul Ilmi -->
    var MasjidBaitulIlmi = L.marker([-5.359054,105.312624]);
    var namaMasjidBaitulIlmi = MasjidBaitulIlmi.bindPopup("Masjid Baitul Ilmi").openPopup()
    namaMasjidBaitulIlmi.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Asrama TB1 -->
    var AsramaTB1 = L.marker([-5.358414,105.317456]);
    var namaAsramaTB1 = AsramaTB1.bindPopup("Asrama TB1").openPopup()
    namaAsramaTB1.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Asrama TB2 -->
    var AsramaTB2 = L.marker([-5.358449,105.319444]);
    var namaAsramaTB2 = AsramaTB2.bindPopup("Asrama TB2").openPopup()
    namaAsramaTB2.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Asrama TB3 -->
    var AsramaTB3 = L.marker([-5.359123,105.319108]);
    var namaAsramaTB3 = AsramaTB3.bindPopup("Asrama TB3").openPopup()
    namaAsramaTB3.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Asrama TB4 -->
    var AsramaTB4 = L.marker([-5.359131,105.317503]);
    var namaAsramaTB4 = AsramaTB4.bindPopup("Asrama TB4").openPopup()
    namaAsramaTB4.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Asrama TB5 -->
    var AsramaTB5 = L.marker([-5.358468,105.318470]);
    var namaAsramaTB5 = AsramaTB5.bindPopup("Asrama TB5").openPopup()
    namaAsramaTB4.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG GSG -->
    var GSG = L.marker([-5.362422,105.318954]);
    var namaGSG = GSG.bindPopup("Gedung Serba Guna").openPopup()
    namaGSG.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG Poliklinik ITERA -->
    var PoliklinikITERA = L.marker([-5.357728,105.315966]);
    var namaPoliklinikITERA = PoliklinikITERA.bindPopup("Poliklinik ITERA").openPopup()
    namaPoliklinikITERA.addTo(map);
	<!-- MENAMPILKAN NAMA ATM ITERA -->
    var ATM_Itera = L.marker([-5.357590,105.315092]);
    var namaATM_Itera = ATM_Itera.bindPopup("ATM ITERA").openPopup()
    namaATM_Itera.addTo(map);
	<!-- MENAMPILKAN NAMA GEDUNG GALERI1 -->
    var Galeri1 = L.marker([-5.357906,105.315573]);
    var namaGaleri1 = Galeri1.bindPopup("Galeri 1 ITERA").openPopup()
    namaGaleri1.addTo(map);
	<!-- MENAMPILKAN NAMA PLTS -->
    var PLTS = L.marker([-5.360436,105.311861]);
    var namaPLTS = PLTS.bindPopup("PLTS ITERA").openPopup()
    namaPLTS.addTo(map);
    var baseMaps = {
	"OSM":osm,
	"ESRI":Esri_WorldImagery,
   };
   var overlayMaps = {
	"Gedung F" : GDGF,
   "Gedung E":GDGE,
   "Embung A": EBGA,
   "Gedung GKU 1" : GKU1,
   "Laboratorium OZT": LaboratoriumOZT,
	"Gedung GKU 2": GKU2,
	"Gedung A" : A,
	"Gedung B" : B,
	"Gedung C dan D" : CdanD,
   "Laboratorium 1": Laboratorium1,
	"Laboratorium 2": Laboratorium2,
	"Laboratorium 3": Laboratorium3,
   "Embung B": EmbungB ,
	"Embung C": EmbungC ,
	"Embung D": EmbungD ,
	"Embung E": EmbungE ,
	"Embung SUMATERA": EmbungSumatera ,
	"LABIRIN" : Labirin ,
    "Kantin BKL": KantinBKL ,
	"Kantin RK": KantinRK ,
	"Rumah Ibadah Multi Agama" : RIMA ,
	"Masjid Raya At-Tanwir" : MasjidRayaAtTanwir ,
	"Masjid Baitul Ilmi" : MasjidBaitulIlmi ,
	"Asrama TB1" : AsramaTB1 ,
	"Asrama TB2" : AsramaTB2 ,
	"Asrama TB3" : AsramaTB3 ,
	"Asrama TB4" : AsramaTB4 ,
	"Asrama TB5" : AsramaTB5 ,
	"Gedung Serba Guna": GSG  ,
	"Poliklinik ITERA" : PoliklinikITERA  ,
   "ATM ITERA": ATM_Itera  ,
	"PLTS ITERA": PLTS   ,
    //"Bundaran GKU": bundaranGKU,
    //"Gedung E": polygon,
   };
   map.removeLayer(GDGF)
   map.removeLayer(GDGE)
   map.removeLayer(EBGA)
   map.removeLayer(GKU1)
   map.removeLayer(LaboratoriumOZT)
   map.removeLayer(GKU2)
   map.removeLayer(A)
   map.removeLayer(B)
   map.removeLayer(CdanD)
   map.removeLayer(Laboratorium1)
   map.removeLayer(Laboratorium2)
   map.removeLayer(Laboratorium3)
   map.removeLayer(EmbungB)
   map.removeLayer(EmbungC)
   map.removeLayer(EmbungD)
   map.removeLayer(EmbungE)
   map.removeLayer(EmbungSumatera)
   map.removeLayer(Labirin)
   map.removeLayer(KantinBKL)
   map.removeLayer(KantinRK)
   map.removeLayer(RIMA)
   map.removeLayer(MasjidRayaAtTanwir)
   map.removeLayer(MasjidBaitulIlmi)
   map.removeLayer(AsramaTB1)
   map.removeLayer(AsramaTB2)
   map.removeLayer(AsramaTB3)
   map.removeLayer(AsramaTB4)
   map.removeLayer(AsramaTB5)
   map.removeLayer(GSG)
   map.removeLayer(PoliklinikITERA)
   map.removeLayer(ATM_Itera)
   map.removeLayer(PLTS)
   //map.removeLayer(bundaranGKU)
   //map.removeLayer(polygon)
   L.control.layers(baseMaps,overlayMaps, {collapsed : false}).addTo(map);
   </script>
