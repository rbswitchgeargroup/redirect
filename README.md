# Redirect Page

This repository contains a simple HTML redirect page.  
Visitors to this page will be redirected to a Microsoft Forms feedback survey.  
If an `email` parameter is present in the URL, it will be logged to an external tracking endpoint before the redirect.

## How it works

- The page reads the `email` query parameter from the URL (e.g. `?email=someone@example.com`).
- If the parameter exists, it sends the email and a timestamp via POST to:  
  `https://yourtrackingendpoint.com/log`
- The user is then redirected to the Microsoft Forms page:
  [Feedback Form](https://forms.office.com/Pages/ResponsePage.aspx?id=35vxefefu02X-mSuwGIMc5eb0pYvMJVLubxnfka86TBUMzRFMVUzVDU3WFQ4OEFNMUNZOVU4QU9VSS4u)

## Usage

1. Clone or download this repository.
2. Edit `redirect.html` to update the tracking endpoint URL if needed.
3. Host the page using GitHub Pages, Netlify, or any web server.
4. Share the link to `redirect.html` with users.  
   You can include `?email=someone@example.com` in the URL to track email addresses.

## Example

```
https://yourusername.github.io/redirect/redirect.html?email=test@example.com
```

## License

No license is currently specified.  
You are welcome to use and modify this page for your own purposes.
