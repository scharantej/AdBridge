## Flask Application Design

### HTML Files

**index.html:**
- Displays a form that allows the user to connect their Meta Business Manager account and Looker Studio.

**success.html:**
- Displayed after a successful connection is established between Meta Business Manager and Looker Studio.

### Routes

**@app.route('/')**
- Renders the index.html file, displaying the connection form.

**@app.route('/connect', methods=['POST'])**
- Handles the form submission, connecting Meta Business Manager and Looker Studio using the provided credentials.
- Redirects to success.html if the connection is successful and displays an error message otherwise.