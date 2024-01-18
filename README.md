 ## Flask Application Design for Snow Forecasting Page

### HTML Files

**1. `index.html`**
- This is the main page of the application.
- It displays the snow forecast for Palisades Tahoe and the expected snowfall on the road from San Francisco to the resort.
- It includes a form that allows users to select a different starting city.

**2. `city.html`**
- This page displays the snow forecast for the selected starting city and the expected snowfall on the road from that city to Palisades Tahoe.

### Routes

**1. `/`**
- This route handles the main page of the application.
- It renders the `index.html` file.

**2. `/city`**
- This route handles the city selection form.
- It retrieves the selected city from the form and redirects to the `/city/<city>` route.

**3. `/city/<city>`**
- This route displays the snow forecast for the selected city and the expected snowfall on the road from that city to Palisades Tahoe.
- It renders the `city.html` file.