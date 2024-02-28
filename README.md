<<<<<<< HEAD
<div align="center">
  <h1 align="center">Open Food Facts Web Scraping API</h1>
  <p align="center">Web scraping API for retrieving product data from Open Food Facts</p>

  ![Project Logo](https://avatars.githubusercontent.com/u/28140896?s=200&v=4)
  ![Open Food Facts Logo](https://static.openfoodfacts.org/images/logos/off-logo-horizontal-light.svg)

  <h2 align="center">Project Overview</h2>

  <p align="center">
    The Open Food Facts Web Scraping API is designed to fetch product information from the Open Food Facts website. It enables users to retrieve details about various products, allowing for filtering based on Nutri-Score and NOVA criteria.
  </p>

  <h2 align="center">Technologies Used</h2>

  - **Puppeteer:** Employed for web scraping on the Open Food Facts website.
  - **Node.js and Express:** Utilized for developing the API.
  - **Swagger:** Integrated for interactive API documentation and testing.
  - **Git Copilot** Used to make code faster and cleaner.
  - **CHAT GPT 4.0**  Used to clarify doubts about the code.

  <h2 align="center">Prerequisites</h2>

  - Download and install Node.js from the [official website](https://nodejs.org/en).

  <h2 align="center">Installation</h2>

  1. **Clone the repository:**
     ```sh
     git clone https://github.com/
     ```
  2. **Install NPM packages:**
     ```sh
     npm install
     ```
  3. **Run the application:**
     ```sh
     node .\app.js
     ```
  4. **Access the API documentation and test it interactively:**
     ```sh
     http://localhost:80/api
     ```

  <h3 align="center">API Endpoints</h3>

  **GET /products**

  - Parameters:
    - `nutrition:` Filter by Nutri-Score (A, B, C, D, E).
    - `nova:` Filter by NOVA score (1, 2, 3, 4, 5).

  - Example:
    ```sh
    curl http://localhost/products?nutrition=A&nova=1
    ```

  **GET /products/{id}**

  - Retrieve detailed product data.
  
  - Parameters:
    - `id:` Product ID.

  - Example:
    ```sh
    curl http://localhost/products/3155250349793
    ```

  <h2 align="center">Scraping Visualization</h2>

  - Inside the `./src/index.js` folder, change `headless` from `true` to `false`:
    ```js
    const browser = await puppeteer.launch({
      headless: false,
      defaultViewport: false,
    });
    ```

  <h2 align="center">Real-time JSON Data Update</h2>

  - Remove the comments that save the products in the JSON files inside the `./src/index.js` folder:
    ```js
    // fs.writeFileSync("./data/products.json", JSON.stringify(products, null, 2));
    // fs.writeFileSync(
    //   "./data/productsDetails.json",
    //   JSON.stringify(productsDetails, null, 2)
    // );
    ```

  <h2 align="center">Contact Information</h2>

  - **Linkedin:** [Guilherme Brasil](https://www.linkedin.com/in/guilherme-brasil-914960273/)
  - **Email:** [guibrasilcontato@gmail.com](mailto:guibrasilcontato@gmail.com)
</div>
