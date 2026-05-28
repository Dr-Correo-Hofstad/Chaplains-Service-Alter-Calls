// AJAX script to calculate Lunar Ephemeris data for Tall el-Hammam
// Coordinates: 31.84° N, 35.67° E (Tall el-Hammam / Jericho region)

function calculateLunarZenith(dateString) {
    // API endpoint for astronomical data (example using a generic Ephemeris API)
    const apiUrl = `https://api.astronomy-data.org/v1/moon-position`;
    
    // Set the parameters for the Middle Bronze Age region
    const params = {
        latitude: 31.84,
        longitude: 35.67,
        date: dateString, // Format: YYYY-MM-DD
        time: "12:00:00"
    };

    // Construct the query string
    const queryString = new URLSearchParams(params).toString();

    // Execute the AJAX request
    console.log(`Calculating moon position for Tall el-Hammam on ${dateString}...`);
    
    fetch(`${apiUrl}?${queryString}`, {
        method: 'GET',
        headers: {
            'Content-Type': 'application/json',
            'Accept': 'application/json'
        }
    })
    .then(response => {
        if (!response.ok) {
            throw new Error(`HTTP error! Status: ${response.status}`);
        }
        return response.json();
    })
    .then(data => {
        // The math/data returned by the astronomical server
        const lunarAltitude = data.altitude; // Degrees above the horizon
        const lunarAzimuth = data.azimuth;   // Compass direction
        
        console.log(`Lunar Altitude: ${lunarAltitude} degrees`);
        console.log(`Lunar Azimuth: ${lunarAzimuth} degrees`);
        
        if (lunarAltitude > 85) {
            console.log("Result: The moon was directly overhead (at zenith) during this time.");
        } else {
            console.log("Result: The moon was NOT directly overhead at this exact time.");
        }
    })
    .catch(error => {
        console.error("AJAX Error calculating lunar position:", error);
    });
}

// Example Execution for a historical date
calculateLunarZenith("-1650-06-15");