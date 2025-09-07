<!-- README.md de Nexor Oficial -->

<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=100&color=gradient&reversal=true" />
<a href="https://emiliano-hn.github.io/Nexor/">
  <img src="Nexor-Data/Nexor-imagenes/Nexor-logo-oficial.png" alt="Logo" width="400" style="margin-top:-10px;" />
</a>
</div>

<p align="center" >𝓓𝓮𝓼𝓲𝓰𝓷𝓮𝓭 𝓯𝓸𝓻 𝓭𝓮𝓿𝓮𝓵𝓸𝓹𝓮𝓻𝓼 𝔀𝓱𝓸 𝓼𝓮𝓮𝓴 𝓮𝓵𝓮𝓰𝓪𝓷𝓬𝓮</p>

<div style="margin-top:40px;">
  <p>QR Tools: </p>
  <a href="https://github.com/user-attachments/files/22061570/Nexor.QR.zip">
    <img src="Nexor-Data/Nexor-imagenes/QR-logo.png" width="150" alt="QR code">
  </a>
</div>

<div style="height:30px;"> </div>

```bash
# Scanning in Nexor v3.0.2 Demo

ble hosts = ["192.168.1.1", "192.168.1.2", "192.168.1.3"]
ble puertos = [22, 80, 443, 8080]
ble resultados = []

fun probar(host, puerto)
    dic (host + ":" + str(puerto)) not in resultados
        ble status = "Closed"
        dic puerto % 2 == 0
            status = "Open"
        nal
        resultados.append(host + ":" + str(puerto) + " → " + status)
    nuf
nuf

fun escaneo_total()
    rp len(hosts)
        ble host = hosts[contador-1]
        rp len(puertos)
            ble puerto = puertos[contador-1]
            probar(host, puerto)
        nuf
    nuf

    Vek "Scan results:"
    rp len(resultados)
        ble linea = resultados[contador-1]
        dic "•" in linea
            Vek "✓" + linea
        nal
            Vek "✗" + linea
    nuf
nuf

escaneo_total()
```

<h1 align="center">Nexor versions:</h1>

<p>Remember that not all versions are final; some may be in testing, incomplete, or contain errors.</p>

<p>
<a href="https://github.com/user-attachments/files/22035692/Nexor.v1.1.0.zip">
  <img src="Nexor-Data/Nexor-imagenes/1.1.0.png" alt="1.1.0" width="65" style="margin-top:-10px;" />
</a>
<a href="https://github.com/user-attachments/files/22035918/Nexor-v1.9.2.zip">
  <img src="Nexor-Data/Nexor-imagenes/1.9.2.png" alt="1.9.2" width="65" style="margin-top:-10px;" />
</a>  
<a href="https://github.com/user-attachments/files/22035929/Nexor-v2.9.3.zip">
  <img src="Nexor-Data/Nexor-imagenes/2.9.3-sf.png" alt="2.9.3" width="65" style="margin-top:-10px;" />
</a> 
<a href="https://github.com/user-attachments/files/22035939/Nexor-v2.9.4.zip">
  <img src="Nexor-Data/Nexor-imagenes/2.9.4.png" alt="2.9.4" width="65" style="margin-top:-10px;" />
</a> 
<a href="https://emiliano-hn.github.io/Nexor/#download">
  <img src="Nexor-Data/Nexor-imagenes/3.0.2.png" alt="3.0.2" width="65" style="margin-top:-10px;" />
</a>   
</p>

<h1 align="center">LICENSE</h1>

<img src="Nexor-Data/Nexor-imagenes/User Responsibility Agreement.png" width="450" height="800" style="border-radius:50%;" alt="Nexor Logo">

<p align="left">Download Document: </p>

<p>
<a href="https://github.com/user-attachments/files/22036534/PNG.zip">
  <img src="Nexor-Data/Nexor-imagenes/PNG.png" alt="PNG" width="65" style="margin-top:-10px;" />
</a>
<a href="https://github.com/user-attachments/files/22036574/PDF.zip">
  <img src="Nexor-Data/Nexor-imagenes/PDF.png" alt="PDF" width="65" style="margin-top:-10px;" />
</a>     
</p>

<div align="center">
   <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=100&color=gradient&section=footer" />
</div>
