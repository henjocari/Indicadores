<html>
	<head>
		<title>Indicadores - Plexa</title>
		<script>
			
			var myVar;
			var indica="https://plexasas-my.sharepoint.com/personal/hcastro_plexa_co/_layouts/15/Doc.aspx?sourcedoc={87791fd9-a02f-40f9-8bfb-7328a38869f1}&action=embedview&wdAllowInteractivity=False&ActiveCell='ABRIL%20CIERRE'!A1&wdHideHeaders=True&wdInConfigurator=True";
			var status="https://plexasas-my.sharepoint.com/personal/trafico_plexa_co/_layouts/15/Doc.aspx?sourcedoc={12b5de58-b899-4c70-b484-42d19ce01788}&action=embedview&wdAllowInteractivity=False&ActiveCell='GLP'!A3&Item=GLP!%C3%81rea_de_impresi%C3%B3n&wdHideGridlines=True&wdInConfigurator=True";
			var statuspgr="https://plexasas-my.sharepoint.com/personal/trafico_plexa_co/_layouts/15/Doc.aspx?sourcedoc={12b5de58-b899-4c70-b484-42d19ce01788}&action=embedview&wdAllowInteractivity=False&ActiveCell='PGR'!A3&Item=PGR!%C3%81rea_de_impresi%C3%B3n&wdHideGridlines=True&wdInConfigurator=True";
			var round="https://plexasas-my.sharepoint.com/personal/hcastro_plexa_co/_layouts/15/Doc.aspx?sourcedoc={44fbcc66-d826-482d-aa6f-759a3cd07c7a}&action=embedview&wdAllowInteractivity=False&ActiveCell='DashBoard'!A1&wdHideGridlines=True&wdHideHeaders=True&wdInConfigurator=True";
			function abrir() {
			  myVar = setTimeout(carga, 180000);
			}

			function carga() {
			  window.open("index.html", "_parent")
			}
			function excel(){
				var aleatorio = Math.round(Math.random()*3);
				if(aleatorio==0){
					document.getElementById('excel').src = indica;
				}
				if(aleatorio==1){
					document.getElementById('excel').src = status;
				}
				if(aleatorio==2){
					document.getElementById('excel').src = round;
				}
				if(aleatorio==3){
					document.getElementById('excel').src = statuspgr;
				}
			}
		</script>
		<style>
			html, body{
				margin: 0;
				padding: 0;
				width: 100%;
				height: 100%;
			}
			iframe{
				
			}
			
		</style>
	</head>
	<body onload="abrir(); excel();">
		<iframe id="excel" width="100%" height="100%" frameborder="0" scrolling="no" src="about:blank"></iframe>
	</body>
</html>
