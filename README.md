<div id="top">

<!-- HEADER STYLE: COMPACT -->

# FB_MARKETPLACE
<em>Automate, Scrape, Analyze: Unleashing Marketplace Data Power</em>

<!-- BADGES -->
<img src="https://img.shields.io/github/license/Rachdyan/fb_marketplace?style=plastic&logo=opensourceinitiative&logoColor=white&color=blueviolet" alt="license">
<img src="https://img.shields.io/github/last-commit/Rachdyan/fb_marketplace?style=plastic&logo=git&logoColor=white&color=blueviolet" alt="last-commit">
<img src="https://img.shields.io/github/languages/top/Rachdyan/fb_marketplace?style=plastic&color=blueviolet" alt="repo-top-language">
<img src="https://img.shields.io/github/languages/count/Rachdyan/fb_marketplace?style=plastic&color=blueviolet" alt="repo-language-count">

<em>Built with the tools and technologies:</em>

<img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=plastic&logo=JavaScript&logoColor=black" alt="JavaScript">
<img src="https://img.shields.io/badge/Selenium-43B02A.svg?style=plastic&logo=Selenium&logoColor=white" alt="Selenium">
<img src="https://img.shields.io/badge/Python-3776AB.svg?style=plastic&logo=Python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=plastic&logo=GitHub-Actions&logoColor=white" alt="GitHub%20Actions">
<img src="https://img.shields.io/badge/pandas-150458.svg?style=plastic&logo=pandas&logoColor=white" alt="pandas">

<br clear="left"/>

## Table of Contents

1. [Table of Contents](#table-of-contents)
2. [Overview](#overview)
3. [Features](#features)
4. [Project Structure](#project-structure)
   <br>&nbsp;&nbsp;&nbsp;&nbsp;4.1. [Project Index](#project-index)
5. [Getting Started](#getting-started)
   <br>&nbsp;&nbsp;&nbsp;&nbsp;5.1. [Prerequisites](#prerequisites)
   <br>&nbsp;&nbsp;&nbsp;&nbsp;5.2. [Installation](#installation)
   <br>&nbsp;&nbsp;&nbsp;&nbsp;5.3. [Usage](#usage)
   <br>&nbsp;&nbsp;&nbsp;&nbsp;5.4. [Testing](#testing)
6. [Roadmap](#roadmap)
7. [Contributing](#contributing)
8. [License](#license)
9. [Acknowledgments](#acknowledgments)


---

## Overview

Harness the power of automation with **fb_marketplace**, a tool that streamlines the process of scraping product listings from Facebook Marketplace, providing a seamless data collection to find deals. The core features include:

- **🤖 Automated Scraping:** Automates the process of scraping product listings, saving you time and effort.
- **📊 Google Sheets Integration:** Exports scraped data directly to Google Sheets for easy data management and analysis.
- **🔔 Real-time Notifications:** Sends notifications about new listings via Telegram, keeping you updated in real-time.
- **🧩 Captcha Solving:** Handles captchas using the 2Captcha service, overcoming a common obstacle in web scraping.
- **🔄 GitHub Actions Workflows:** Automates the execution of the scraping script in different environments, ensuring regular data collection.

---

## Features

|      | Component       | Details                              |
| :--- | :-------------- | :----------------------------------- |
| ⚙️  | **Architecture**  | <ul><li>Written in Python and JavaScript</li><li>Uses Selenium for web scraping</li><li>Utilizes PyDrive2 for Google Drive operations</li></ul> |
| 🔩 | **Code Quality**  | <ul><li>Consistent use of Python best practices</li><li>Well-structured JavaScript code</li><li>Use of linters for code quality assurance</li></ul> |
| 📄 | **Documentation** | <ul><li>No dedicated documentation found</li><li>Code comments provide some level of documentation</li></ul> |
| 🔌 | **Integrations**  | <ul><li>Integrated with GitHub Actions for CI/CD</li><li>Uses 2captcha for captcha solving</li><li>Integration with Telegram for notifications</li></ul> |
| ⚡️  | **Performance**   | <ul><li>Efficient use of Python libraries for data handling</li><li>Performance may vary based on web scraping speed</li></ul> |
| 🛡️ | **Security**      | <ul><li>Use of python-dotenv for environment variable management</li><li>2captcha used for captcha challenges</li></ul> |
| 📦 | **Dependencies**  | <ul><li>Managed through pip with requirements.txt</li><li>Dependencies include pandas, selenium, BeautifulSoup4, etc.</li></ul> |
| 🚀 | **Scalability**   | <ul><li>Scalability dependent on the efficiency of the web scraping process</li><li>Use of Google Drive for storage provides scalability</li></ul> |

---

## Project Structure

```sh
└── fb_marketplace/
    ├── .github
    │   └── workflows
    ├── js_scripts
    │   ├── get_captcha_data.js
    │   └── track_image_updates.js
    ├── requirements.txt
    ├── scrape_marketplace.py
    └── utils
        ├── __init__.py
        ├── __pycache__
        ├── captcha_utils.py
        ├── fb.py
        ├── gsheet_utils.py
        └── telegram_utils.py
```

### Project Index

<details open>
	<summary><b><code>FB_MARKETPLACE/</code></b></summary>
	<!-- __root__ Submodule -->
	<details>
		<summary><b>__root__</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ __root__</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/requirements.txt'>requirements.txt</a></b></td>
					<td style='padding: 8px;'>- Requirements.txt outlines the necessary Python libraries for the project, ensuring consistent environments across setups<br>- It includes libraries for web scraping (beautifulsoup4, lxml), Google Sheets interaction (gspread, gspread_dataframe), automation (pyautogui), Google Drive access (PyDrive2), environment variable management (python-dotenv), Telegram bot creation (python-telegram-bot), date manipulation (python_dateutil), web testing (selenium, seleniumbase), OTP generation (pyotp), and captcha solving (2captcha-python).</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/scrape_marketplace.py'>scrape_marketplace.py</a></b></td>
					<td style='padding: 8px;'>- The <code>scrape_marketplace.py</code> script automates the process of scraping product listings from Facebook Marketplace<br>- It logs into Facebook, navigates to the marketplace, and searches for specific products<br>- The script then filters new listings, compares them with previously scraped data, and exports the new listings to a Google Sheet<br>- It also sends notifications about new listings via Telegram.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- utils Submodule -->
	<details>
		<summary><b>utils</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ utils</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/utils/fb.py'>fb.py</a></b></td>
					<td style='padding: 8px;'>- The <code>fb.py</code> utility module in the project is primarily responsible for scraping product data from Facebook Marketplace<br>- It extracts product details such as title, link, price, image link, and location, and organizes this data into a Pandas DataFrame<br>- Additionally, it provides functionality to search the marketplace based on specific product criteria.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/utils/captcha_utils.py'>captcha_utils.py</a></b></td>
					<td style='padding: 8px;'>- CaptchaUtils provides a set of classes and methods for interacting with captchas and executing JavaScript code through Selenium WebDriver<br>- It enables the automation of captcha solving using the 2Captcha service, handling of error messages, and interaction with page elements<br>- The code also facilitates the execution of JavaScript within the browser context.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/utils/gsheet_utils.py'>gsheet_utils.py</a></b></td>
					<td style='padding: 8px;'>- Gsheet_utils.py serves as a utility module for interacting with Google Sheets<br>- It provides functionality to export data to a specified sheet, with options to write or append data, and retrieve data from a sheet<br>- This module plays a crucial role in data management within the projects architecture.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/utils/telegram_utils.py'>telegram_utils.py</a></b></td>
					<td style='padding: 8px;'>- TelegramUtils serves as a utility module in the project, primarily responsible for generating and sending formatted messages via Telegram<br>- It leverages the Telegram API to send messages, and handles any exceptions that may occur during this process<br>- The messages are constructed using data from a pandas Series, including details like link, title, price, location, and original keyword.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- js_scripts Submodule -->
	<details>
		<summary><b>js_scripts</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ js_scripts</b></code>
			<table style='width: 100%; border-collapse: collapse;'>
			<thead>
				<tr style='background-color: #f8f9fa;'>
					<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
					<th style='text-align: left; padding: 8px;'>Summary</th>
				</tr>
			</thead>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/js_scripts/get_captcha_data.js'>get_captcha_data.js</a></b></td>
					<td style='padding: 8px;'>- GetCaptchaData, located in js_scripts/get_captcha_data.js, is a JavaScript function that retrieves reCAPTCHA data from a webpage<br>- It creates a canvas, extracts the reCAPTCHA image and description, and returns this data as a promise<br>- The function supports both 3x3 and 4x4 reCAPTCHA grids, making it versatile for different website configurations.</td>
				</tr>
				<tr style='border-bottom: 1px solid #eee;'>
					<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/js_scripts/track_image_updates.js'>track_image_updates.js</a></b></td>
					<td style='padding: 8px;'>- Monitoring and identifying specific image update requests is the primary function of track_image_updates.js within the codebase<br>- It observes performance entries for XMLHttpRequest or Fetch initiated requests, specifically targeting those containing recaptcha/api2/replaceimage in their URL<br>- After a 10-second interval, it returns a promise resolving to a flag indicating the presence of such requests.</td>
				</tr>
			</table>
		</blockquote>
	</details>
	<!-- .github Submodule -->
	<details>
		<summary><b>.github</b></summary>
		<blockquote>
			<div class='directory-path' style='padding: 8px 0; color: #666;'>
				<code><b>⦿ .github</b></code>
			<!-- workflows Submodule -->
			<details>
				<summary><b>workflows</b></summary>
				<blockquote>
					<div class='directory-path' style='padding: 8px 0; color: #666;'>
						<code><b>⦿ .github.workflows</b></code>
					<table style='width: 100%; border-collapse: collapse;'>
					<thead>
						<tr style='background-color: #f8f9fa;'>
							<th style='width: 30%; text-align: left; padding: 8px;'>File Name</th>
							<th style='text-align: left; padding: 8px;'>Summary</th>
						</tr>
					</thead>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/.github/workflows/scrape_mp.yml'>scrape_mp.yml</a></b></td>
							<td style='padding: 8px;'>- Scrape Marketplace is a GitHub Actions workflow that automates the process of scraping data from an online marketplace<br>- It sets up a Python environment, installs necessary dependencies, and runs the scraping script<br>- The workflow is designed to run on an Ubuntu 22.04 operating system and uses secrets for secure data handling.</td>
						</tr>
						<tr style='border-bottom: 1px solid #eee;'>
							<td style='padding: 8px;'><b><a href='https://github.com/Rachdyan/fb_marketplace/blob/master/.github/workflows/scrape_mp_windows.yml'>scrape_mp_windows.yml</a></b></td>
							<td style='padding: 8px;'>- Scrape Marketplace Windows is a GitHub Actions workflow that automates the execution of a Python script on a Windows environment<br>- It is scheduled to run daily, setting up the necessary Python environment, installing dependencies, and executing the <code>scrape_marketplace.py</code> script<br>- This workflow contributes to the project by ensuring regular data scraping from the marketplace.</td>
						</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
</details>

---

## Getting Started

### Prerequisites

This project requires the following dependencies:

- **Programming Language:** Python
- **Package Manager:** Pip

### Installation

Build fb_marketplace from the source and intsall dependencies:

1. **Clone the repository:**

    ```sh
    ❯ git clone https://github.com/Rachdyan/fb_marketplace
    ```

2. **Navigate to the project directory:**

    ```sh
    ❯ cd fb_marketplace
    ```

3. **Install the dependencies:**



	```sh
	❯ pip install -r requirements.txt
	```

### Usage

Run the project with:

**Using [pip](https://pypi.org/project/pip/):**
```sh
python {entrypoint}
```


---

## Contributing

- **💬 [Join the Discussions](https://github.com/Rachdyan/fb_marketplace/discussions)**: Share your insights, provide feedback, or ask questions.
- **🐛 [Report Issues](https://github.com/Rachdyan/fb_marketplace/issues)**: Submit bugs found or log feature requests for the `fb_marketplace` project.
- **💡 [Submit Pull Requests](https://github.com/Rachdyan/fb_marketplace/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/Rachdyan/fb_marketplace
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to github**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details closed>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://github.com{/Rachdyan/fb_marketplace/}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=Rachdyan/fb_marketplace">
   </a>
</p>
</details>

---

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.


---

## Disclaimer

This is a personal project developed solely for educational and personal use.


[back-to-top]: https://img.shields.io/badge/-BACK_TO_TOP-151515?style=flat-square


---
