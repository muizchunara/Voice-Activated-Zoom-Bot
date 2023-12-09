


<h3 align="center">Voice Activated Zoom Bot using Recall.AI</h3>

  <p align="center">
    Using the live zoom call transcribing provided by Recall.AI, this bot can be setup to listen for key words then perform a specified action including calling an external API, in the example provided the Bot will call Dalle-3 to generate an image then drop that image in the Zoom Call

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Here is a framework to help you create your own Zoom Bots using Recall.AI that can listen for keyword based voice commands and perform actions in the call, this can be especially useful when combined with content fetching/generating APIs like Google Drive or Dalle-3

Voice activated commands can help to streamline zoom calls by preventing the need for the host or speaker to leave their zoom client to go looking for files, or to drop links into the Zoom call, instead being able to have a bot do it for them using just their voice

### Built With

Python
Recall.AI

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites
* A Recall.AI API Key
* A Gladia API Key

### Installation

1. Get a Recall.AI API Key at [https://recall.ai](https://recall.ai)
2. Get a Gladia API Key at [https://gladia.io](gladia.io)
3. Add your Gladia API Key to your Recall account using the API Dashboard
4. Clone the repo
   ```sh
   git clone https://github.com/github_username/repo_name.git
   ```
5. Install Python packages
   ```sh
   pip install requirements.txt
   ```
6. Enter your API in `app.py	`
   ```py
   RECALL_KEY="YOUR_RECALLAI_API_KEY_HERE"
   ```
7. Set a keyword to trigger the voice command in `app.py	`
	 ```py
   trigger="SET YOUR VOICE COMMAND TRIGGER"
   ```
 8. Add any commands or tasks you may want to run following the voice command in `app.py	`

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

1. Run `app.py`
2. Direct the Recall.AI Webhook endpoint to your running service
3. Send a bot creation webhook to your service `{"create-bot: MEETING_URL"}`
4. The bot will automatically begin working once the recording start webhook is received from Recall.AI
5. The bot will automatically stop once the done webhook is received from Recall.AI

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>





