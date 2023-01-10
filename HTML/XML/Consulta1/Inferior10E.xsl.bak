<?xml version="1.0" encoding="UTF-8"?>
<xsl:stylesheet version="1.0" xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
<xsl:template match="/">
	<html>
	<head>
		<meta charset="utf-8"/>
		<title>consultas juegos inferiores a 15euro</title>
		<style type="text/css">
			h1{
				color:black;
				text-align:center;
				font-size:50px;
				font-family:fantasy;
				text-shadow: 5px 5px 5px white;
			} 
			table{
				margin:auto;
				font-size:20px;
				align :center;
				border:1px collapse blue;
				box-shadow: 5px 10px 8px #888888;
				border-radius: 5px;
				padding:10px;
				border-spacing:5px;
				width:80%;
			}
			td:hover{
			background-color:lime;
			}
		</style>
	</head>
		<body>			
			<h1>consultas juegos superior a 15 euro</h1>
			<div>
				<table border ="2">
					<tr style="background:00FF8F">
						<th> NOMBRE </th>
						<th> PRECIO </th>
						<th> FECHA LANZAMIENTO </th>
					</tr>
					<xsl:for-each select="Juegos/juego">
						<xsl:sort select="precio" order="ascending"/>
						<xsl:if test="precio > 15">	
							<tr>
								<td><xsl:value-of select="nombre"/></td>
								<td><xsl:value-of select="precio"/>€</td>
								<td><xsl:value-of select="//anio"/>-<xsl:value-of select="//mes"/>-<xsl:value-of select="//dia"/></td>
							</tr>
						</xsl:if>
					</xsl:for-each>
				</table>
			</div>
		</body>
	</html>	
</xsl:template>
</xsl:stylesheet>