# location-finder
<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Location Finder</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: #f4f4f4;
        }
        .container {
            max-width: 900px;
            margin: auto;
            padding: 20px;
        }
        h1 {
            text-align: center;
            margin-bottom: 20px;
        }
        #map {
            width: 100%;
            height: 400px;
            background: #ccc;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .contact-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 10px;
        }
        .contact-item {
            background: white;
            padding: 15px;
            border-radius: 10px;
            cursor: pointer;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: 0.3s;
        }
        .contact-item:hover {
            background: #d7ebff;
        }
        #my-location-btn {
            width: 100%;
            padding: 15px;
            background: #007bff;
            color: white;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            font-size: 18px;
            margin-bottom: 10px;
        }
        #my-location-btn:hover {
            background: #0068d6;
        }
        #status {
            text-align: center;
            margin-top: 10px;
            font-weight: bold;
        }
    </style><link
    rel="stylesheet"
    href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
/>

</head>
<body>
    <div class="container">
        <h1>Location Finder</h1><button id="my-location-btn">Show My Location</button>
    <div id="status"></div>

    <div id="map"></div>

    <h2>Saved Locations</h2>
    <div class="contact-list">
        <div class="contact-item" data-lat="28.6139" data-lon="77.2090" data-name="Delhi">Delhi</div>
        <div class="contact-item" data-lat="19.0760" data-lon="72.8777" data-name="Mumbai">Mumbai</div>
        <div class="contact-item" data-lat="13.0827" data-lon="80.2707" data-name="Chennai">Chennai</div>
        <div class="contact-item" data-lat="12.9716" data-lon="77.5946" data-name="Bengaluru">Bengaluru</div>
    </div>
</div>

<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script>
    let map = L.map('map').setView([20.5937, 78.9629], 5);

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: 'Map data © OpenStreetMap contributors'
    }).addTo(map);

    let marker;

    function showLocation(lat, lon, name, zoomIn) {
        if (marker) {
            map.removeLayer(marker);
        }

        marker = L.marker([lat, lon]).addTo(map).bindPopup(name).openPopup();

        map.setView([lat, lon], zoomIn ? 14 : 10);

        document.getElementById('status').innerText = "Showing: " + name;
    }

    // Event listener for all contact items
    document.querySelectorAll('.contact-item').forEach(item => {
        item.addEventListener('click', function () {
            const lat = parseFloat(this.dataset.lat);
            const lon = parseFloat(this.dataset.lon);
            const name = this.dataset.name;
            showLocation(lat, lon, name, false);
        });
    });

    // My Location Button
    document.getElementById('my-location-btn').addEventListener('click', function () {
        if (!navigator.geolocation) {
            document.getElementById('status').innerText = "Geolocation not supported.";
            return;
        }

        document.getElementById('status').innerText = "Locating you...";

        navigator.geolocation.getCurrentPosition(
            function (position) {
                const lat = position.coords.latitude;
                const lon = position.coords.longitude;
                showLocation(lat, lon, "Your Location", true);
            },
            function (error) {
                document.getElementById('status').innerText = "Error: " + error.message;
                showLocation(28.6139, 77.2090, "Fallback Demo (Delhi)", true);
            }
        );
    });
</script>

</body>
</html>
