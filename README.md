# BF1-Live-Server-Banner
Dynamically generate image with BF1 server information in real-time in PHP using battlefieldtracker API JSON data.


# Installation Instructions
1) Upload "sig.php" and "/media" directory to web server.
2) Obtain an API key from https://battlefieldtracker.com/site-api
3) Open up "sig.php" and replace _YOUR_API_KEY_ with your battletracker API key inside of `getData()` function (in  curl_setopt($ch, CURLOPT_HTTPHEADER....)


When additional maps are released, you'll need to add new background canvas images containing a thumbnail picture of the map into the `/media/img_canvas/` directory. The GIMP image template titled "banner template.xcf" is included in this directory.

Warning: If testing this on a local Windows-based Apache server (e.g., XAMPP), you'll need to add the SSL sertificate per directions here: http://stackoverflow.com/questions/29822686/curl-error-60-ssl-certificate-unable-to-get-local-issuer-certificate
