# Scalable Data Migration from PostgreSQL to MySQL Database
<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
 

<div id="top"></div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <h3 align="center">Data Warehousing</h3>

  <p align="center">
    A dockerized ELT pipeline.
    <br /><br />
    <a href="https://traffic-doc.netlify.app/"><strong>Explore the docs »</strong></a>
    <br /> 
    <a href="https://github.com/bkget/Scalable-Data-Migration/issues">Report Bug</a>
    ·
    <a href="https://github.com/bkget/Scalable-Data-Migration/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details open="open">
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
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project
![alt text](https://github.com/bkget/Scalable-Data-Migration/blob/main/screenshots/migration_architecture.png?raw=true)
A dockerized Extract, Load, Transform (ELT) pipeline with PostgreSQL, Airflow, DBT, and a Redash.

### Built With

Tech Stack used in this project includes:
* [![Docker][Docker.com]][Docker-url]
* [![Postgres][Postgresql.com]][Postgresql-url]
* [![Airflow][Airflow.com]][Airflow-url]
* [![DBT][DBT.com]][DBT-url]
* [![Superset][Superset.com]][Superset-url]

<!-- GETTING STARTED -->
## Getting Started
### Prerequisites
Make sure you have docker installed on local machine.
-   Docker
-   Docker Compose

### Installation

1. Clone the repo
    ```sh
    git clone https://https://github.com/bkget/Scalable-Data-Migration.git
    ```
2. Navigate to the folder
    ```sh
    cd Scalable-Data-Migration
    ```
3. Build an airflow image
    ```sh
    docker build . --tag apache_dbt/airflow:2.3.3
    ```
4. Run
    ```sh
     docker-compose up
    ```
5. Open Airflow web browser
    ```JS
    Navigate to `http://localhost:8080/` on the browser
    activate and trigger load_dag
    activate and trigger dbt_dag
    ```
6. Access redash dashboard
    ```JS
    Navigate to `http://localhost:5000/` on the browser
    ```

<!-- CONTRIBUTING -->
## Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License
Distributed under the MIT License. See `LICENSE` for more information.

<!-- CONTACT -->
## Contact
Biruk Getaneh - bkgetmom@gmail.com

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments
-   [10 Academy](https://www.10academy.org/)

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/bkget/Scalable-Data-Migration.svg?style=for-the-badge
[contributors-url]: https://github.com/bkget/Scalable-Data-Migration/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/bkget/Scalable-Data-Migration?style=for-the-badge
[forks-url]: https://github.com/bkget/Scalable-Data-Migration?style=for-the-badge
[stars-shield]: https://img.shields.io/github/stars/bkget/Scalable-Data-Migration?style=for-the-badge
[stars-url]: https://github.com/bkget/Scalable-Data-Migration/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/bkget/Scalable-Data-Migration/issues?style=for-the-badge
[license-shield]: https://img.shields.io/github/license/bkget/Scalable-Data-Migration?style=for-the-badge
[license-url]: https://github.com/bkget/Scalable-Data-Migration/blob/main/LICENSE
[Postgresql.com]: https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white
[Postgresql-url]: https://www.postgresql.org/
[Airflow.com]: https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=Apache%20Airflow&logoColor=white
[Airflow-url]: https://airflow.apache.org/
[Docker.com]: https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com/
[DBT.com]: https://img.shields.io/badge/DBT-FF694B?style=for-the-badge&logo=dbt&logoColor=white
[DBT-url]: https://docs.getdbt.com/ 
[DBT.com]: https://img.shields.io/badge/superset-FF694B?style=for-the-badge&logo=superset&logoColor=white
[Superset-url]: https://superset.apache.org/
