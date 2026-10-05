# ANRYZO digital business card

A single-page, mobile-first Flask site with tap-to-call, email, and Instagram links. The supplied Anryzo logo is included in `static/anryzo-logo.jpeg`.

## Run it locally

1. Install Python 3.10 or newer.
2. In this folder, install dependencies with `pip install -r requirements.txt`.
3. Start the site with `python app.py` and open `http://127.0.0.1:5000`.

## Publish on Render

1. Put the `anryzo-card` folder in a GitHub repository and push it to GitHub.
2. In Render, choose **New + → Blueprint** and connect that repository. Render reads `render.yaml` to install the dependencies and start the Flask site.
3. After the deploy succeeds, open the `onrender.com` URL Render assigns and check the page and all three contact links on your phone.
4. If the repository contains several projects, set the Render service's **Root Directory** to `anryzo-card` (or place these files at the repository root before connecting it).

## Make the business-card QR code

After deployment, copy the complete public HTTPS URL Render gives you (for example, `https://anryzo-card.onrender.com`). Use that URL as the QR code destination in your preferred QR-code generator, then scan the finished code with a phone before printing. The QR points to this page, so you can update the contact details on the site later without changing the printed code.

Keep the deployed URL active for as long as the printed cards are in circulation. If you later connect a custom domain, you can use that domain for future QR codes.
