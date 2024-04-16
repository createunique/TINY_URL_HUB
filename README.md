# URL SHORTENER

## Overview
The URL Shortener project offers a user-friendly solution for shortening long URLs into concise and shareable links. With its simple web interface, users can effortlessly input lengthy URLs and receive shortened versions, streamlining the process of link distribution and sharing across various platforms.

## How to Use
1. **Input Long URL:** Start by entering the long URL that you wish to shorten into the designated input field provided on the web page.
2. **Click Shorten:** Once you've entered the long URL, proceed to click the "Shorten" button to initiate the shortening process.
3. **Copy Shortened URL:** After the shortening process is complete, the shortened URL will be generated and displayed on the page. You can then conveniently copy it to your clipboard using the "Copy" button provided for easy sharing.

## Working Mechanism
The URL Shortener functions through a series of systematic steps:

- **User Input:** Users interact with the URL Shortener by entering a long URL into the provided input field on the web interface. This input field serves as the entry point for the URL shortening process.

- **Validation:** Upon submission of the long URL, the input undergoes validation to ensure it conforms to a proper URL format. This validation step is crucial for maintaining the integrity and accuracy of the shortening process. Validation checks may include verifying the presence of essential components such as the protocol (e.g., HTTP, HTTPS), domain name, and path.

-**Shortening Process:** After successful validation, the URL Shortener proceeds to shorten the long URL by generating a unique shortened version. This process typically involves utilizing a hashing algorithm, such as SHA-256, to create a compact representation of the original URL. The SHA-256 hashing algorithm generates a fixed-length hash value based on the input data (i.e., the long URL), providing a distinct identifier for the URL while maintaining data integrity and security.

-**Database Storage:** Once the shortened URL is generated, both the original long URL and its corresponding shortened version are securely stored in a MySQL database. This database serves as a centralized repository for managing URL data efficiently. Storing URLs in a database enables seamless retrieval and management of URL records, facilitating future access and manipulation as needed. Database storage ensures that the URL Shortener can handle large volumes of URLs while maintaining performance and scalability.

-**Return Shortened URL:** Upon successful completion of the shortening process and database storage, the shortened URL is promptly returned to the user. This shortened URL serves as a concise and shareable representation of the original long URL. Users can then copy the shortened URL from the web interface and utilize it for various purposes, such as sharing links on social media, embedding in emails, or posting on websites. The prompt return of the shortened URL enhances user experience by providing instant access to the shortened link, facilitating seamless sharing and dissemination across different platforms.

## Files & Components
- `index.html`: This HTML file serves as the primary interface for users to input long URLs and view shortened versions.
- `shorten.php`: The PHP script responsible for processing long URLs, generating shortened versions, and securely storing them in the MySQL database.
- `redirect.php`: This PHP script manages the redirection of shortened URLs to their original long versions, ensuring seamless navigation for users.
- `styles.css`: The CSS file containing styles to enhance the visual presentation and user experience of the web interface.
- `script.js`: JavaScript functionalities incorporated into this file handle client-side validation and user interaction, contributing to a smoother and more responsive user experience.

## User Interface
The user interface of the URL Shortener project is designed with simplicity and functionality in mind:
- **Input Field:** Users can effortlessly input long URLs into the designated input field, providing a seamless experience.
- **Shorten Button:** A single click on the "Shorten" button initiates the shortening process, simplifying the overall interaction flow.
- **Shortened URL Display:** The shortened URL is prominently displayed to users upon generation, accompanied by a convenient "Copy" button for effortless sharing and dissemination.
