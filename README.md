# AR-CITY-WEB-APP 

## An OpenARCloud-based system to accurately and remotely place objects to previously scanned reconstructions ##

#### Previously, reconstructions produced by OpenARCloud's AC-Scanner app, required the AC-Objects app to manually be within a location and place a sticker to that location. Now, with our new system, users are able to post stickers remotely to a previously scanned reconstruction, without needing to be anywhere near the post location, as long as an initial object has been placed in the reconstruction before. ####

To get started, and use our web app, please follow the steps below:

1. Our system integrates the Google Maps API to calculate our location data. To use this API, head to the [Google Maps Platform Credentials page](https://console.cloud.google.com/project/_/google/maps-apis/credentials "Google Maps Platform Credentials page") to produce an API key - this is free but is required since keeping the use of APIs restricted only to authorised API keys adds security to the application, and ensures requests can only be made with your specific API key.

2. Follow the steps on their website until an API key for your project has been generated

3. Find the following code block on line 169 in sample.html, and enter your unique API key in place for [YOUR_API_KEY]:

          <script
                src="https://maps.googleapis.com/maps/api/js?key=[YOUR_API_KEY]&callback=initMap&v=weekly"
                async>
          </script>

4. The web app is now ready to use. Save sample.html and open it in your browser

5. To remotely post an object to a reconstruction, find the desired post location on the map, enter an object name and an object description. The radius can be manipulated to specify how far from the marked location the API should search for reconstruction IDs. The system will alert the user to confirm the post was successful or unsuccessful
          
