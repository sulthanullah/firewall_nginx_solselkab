<div id="top"></div>
<!--
*** Thanks for checking out the Best Sulthanullah. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="#">
    <img src="images/Lambang_Kabupaten_Solok_Selatan.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Nginx firewal lsolselkab</h3>

  <p align="center">
    OpenSource Firewall
    <br />
    <a href="#"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="#">View Demo</a>
    ·
    <a href="#">Report Bug</a>
    ·
    <a href="#">Request Feature</a>
  </p>
</div>



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
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]]()




<p align="right">(<a href="#top">back to top</a>)</p>



### Tech Stack

CKAN dikembangkan dengan menggunakan bahasa pemrograman Python sebagai backend, JavaScript sebagai frontend, database PostgreSQL dan search engine Solr. CKAN memungkinkan untuk ditambahkan ekstensi atau fitur tambahan karena memakai arsitektur modular. Selain itu CKAN juga memiliki fitur API.

* [Python](https://www.python.org/downloads/)
* [PostgreSQL](https://www.jetbrains.com/datagrip/features/?source=google&medium=cpc&campaign=15034928131&gclid=Cj0KCQiA09eQBhCxARIsAAYRiym4GpmfEQVKxJR41HXWfTV4lA1QN0q9-SPzHS1RVQN4CAPbVjqkv4EaArViEALw_wcB)
* [Solr](https://en.wikipedia.org/wiki/Apache_Solr)
* [Ubuntu](https://ubuntu.com)
* [Docker](http://docker.com)
* [Proxmox](https://www.proxmox.com/en/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

* Install Proxmox
* Install VM Ubuntu
* Install Docker
* Git Clone CKAN


### Prerequisites

- 👨‍💻 &nbsp; Step One
* Update Ubuntu
  ```sh
  apt update
  ```
* Upgrade Ubuntu
  ```sh
  apt upgrade -y
  ```
* Install alat bantu 
  ```sh
  apt-get install python3 python3-setuptools docker.io -y
  ```
* Install pip3
  ```sh
  apt-get install python3-pip -y
  ```
* Install curl
  ```sh
  apt-get install curl -y
  ```
  
### Installation

_Langkah - Langkah Install CKAN In Proxmox._

1. Upgrade docker-compose version
     ```sh
   sudo apt-get remove docker-compose
   ```
      ```sh
   sudo curl -L "https://github.com/docker/compose/releases/download/1.23.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
   ```
     ```sh
   sudo chmod +x /usr/local/bin/docker-compose
   ```
      ```sh
   sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
   ```
2. Clone the repo
   ```sh
   git clone https://github.com/ckan/ckan.git
   ```
3. Install
   ```sh
   git checkout tags/ckan-2.9.0
   ```
      ```sh
   cd /ckan/contrib/docker
   ```
      ```sh
   cp -rp .env.template .env
   ```
      ```sh
     docker-compose up -d --build
   ```
4. Check the installation successfully completed
      ```sh
     docker-compose restart ckan
   ```
    ```sh
     docker ps | grep ckan
   ```
     ```sh
     docker-compose logs -f ckan
   ```
5. Access to your site_url domain or IP.
   ```js
     http://{site_url_domain or IP}:5000
   ```

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact <a href="https://www.gautamkrishnar.com/"><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px"></a>

<p align="left">
<a href="#" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/dev-dot-to.svg" alt="gautamkrishnar" height="30" width="40" /></a>
<a href="#" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="gautamkrishnar" height="30" width="40" /></a>
<a href="#" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="gautamkrishnar" height="30" width="40" /></a>
<a href="#" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/stack-overflow.svg" alt="4214976" height="30" width="40" /></a>
<a href="#" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="gautamkrishnar" height="30" width="40" /></a>

Project Link: [https://github.com/sulthanullah](https://github.com/sulthanullah)

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
