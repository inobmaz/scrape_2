
Web Page Content Fetcher
This script demonstrates how to use Python's urllib.request module to fetch and display the HTML content of a web page.

Features
Connects to a given URL.
Reads the HTML content from the web page.
Decodes the HTML content to a human-readable string.
Prints the HTML to the console.
Requirements
Python 3.x
Internet connection
Code Explanation
python
Copy code
from urllib.request import urlopen

url = "http://olympus.realpython.org/profiles/aphrodite"  # URL of the web page to fetch
page = urlopen(url)                                      # Opens the URL
html_bytes = page.read()                                 # Reads the raw HTML content
html = html_bytes.decode("utf-8")                        # Decodes the HTML to a string

print(html)                                              # Prints the HTML content
Key Steps:
Importing Libraries:

The script uses urllib.request to handle HTTP requests.
Specifying the URL:

Replace the URL with any desired web page URL to fetch its content.
Fetching the Page:

The urlopen() function connects to the URL and retrieves the page content.
Decoding Content:

The content is decoded from raw bytes into a UTF-8 encoded string.
Displaying Output:

The HTML is printed to the console for inspection.
How to Use
Clone or download this script.

Ensure you have Python 3 installed on your system.

Run the script in your terminal or Python IDE:

bash
Copy code
python fetch_html.py
The HTML content of the web page will be displayed in your console.

Notes
The target website must be accessible for the script to work.
Be mindful of the site's terms of service when fetching content.
This script is for educational purposes and demonstrates basic web scraping techniques.
Potential Enhancements
Save the HTML content to a file for offline use.
Parse the HTML using libraries like BeautifulSoup for data extraction.
Add error handling for scenarios like unavailable URLs or network issues.
Enjoy exploring the world of web scraping! 😊
