<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSXPq_MLAo5At7AN38bw8O6baOmoV6lJeBJdKUDH6YD09R4FEwLNMO5v7utvifuTCrVFqU&usqp=CAU" width="100" alt="project-logo">
</p>
<p align="center">
    <h1 align="center">OCULUS-2022-BE</h1>
</p>
<p align="center">
    <em>Architecting seamless experiences, forging limitless connections.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/last-commit/kashishvjain/Oculus-2022-be?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/kashishvjain/Oculus-2022-be?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/kashishvjain/Oculus-2022-be?style=default&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
	<!-- default option, no dependency badges. -->
</p>

<br><!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary><br>

- [ Overview](#-overview)
- [ Features](#-features)
- [ Repository Structure](#-repository-structure)
- [ Modules](#-modules)
- [ Getting Started](#-getting-started)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
  - [ Tests](#-tests)
- [ Project Roadmap](#-project-roadmap)
- [ Contributing](#-contributing)
- [ License](#-license)
- [ Acknowledgments](#-acknowledgments)
</details>
<hr>

##  Overview

Oculus-2022-be is a robust open-source project offering a sophisticated backend infrastructure for the Oculus application. This software project facilitates seamless user interactions by managing data flow, API endpoints, and Firebase integration. Through Django and Django REST framework, Oculus-2022-be empowers efficient event data retrieval, team updates, and secure payment processes. The repositorys structured architecture, interactive notifications, and robust testing mechanisms reflect its commitment to delivering a reliable and scalable platform for the Oculus community.

---

##  Features

|    |   Feature         | Description |
|----|-------------------|---------------------------------------------------------------|
| ⚙️  | **Architecture**  | Django-based project utilizing Firebase for backend services. Follows a typical Django architecture with models, views, and admin interface. Supports asynchronous server applications. |
| 🔩 | **Code Quality**  | Codebase follows Django best practices. Well-structured code with clear separation of concerns. Maintains PEP 8 standards for Python code consistency. |
| 🔌 | **Integrations**  | Integrates Firebase for authentication and external API services. Dependencies include Django, Django REST framework for API development. |
| 🧩 | **Modularity**    | Codebase is modular with separate apps for different functionalities. Supports easy scalability and maintenance. Follows Django app structure for reusability. |
| 🧪 | **Testing**       | Utilizes Django's test framework for unit testing. Tests cover API functionality ensuring reliability and stability. Could expand test coverage for broader scenarios. |
| ⚡️  | **Performance**   | Efficient performance with Django's built-in optimizations. Utilizes Firebase for real-time updates and data synchronization. Resource usage is optimized and scales well. |
| 🛡️ | **Security**      | Secure handling of sensitive data with Firebase service account credentials. Follows Django security best practices for data protection and access control. |
| 📦 | **Dependencies**  | Key dependencies include Django, Django REST framework, Firebase, and Pandas for data processing. Manages dependencies using Pipfile and Pipfile.lock. |
| 🚀 | **Scalability**   | Designed for scalability with Django's scalability features and Firebase's real-time database capabilities. Can handle increased traffic and load effectively. |

---

##  Repository Structure

```sh
└── Oculus-2022-be/
    ├── APIserver
    │   ├── __init__.py
    │   ├── __pycache__
    │   ├── admin.py
    │   ├── apps.py
    │   ├── credentials.json
    │   ├── files
    │   ├── models.py
    │   ├── tests.py
    │   ├── urls.py
    │   └── views.py
    ├── OculusSite
    │   ├── __init__.py
    │   ├── __pycache__
    │   ├── asgi.py
    │   ├── credentials.json
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    ├── Pipfile
    ├── Pipfile.lock
    ├── Procfile
    ├── db.sqlite3
    ├── manage.py
    └── requirements.txt
```

---

##  Modules

<details closed><summary>.</summary>

| File                                                                              | Summary                                                                                                                                                                                              |
| ---                                                                               | ---                                                                                                                                                                                                  |
| [manage.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/manage.py) | Executes Django admin tasks, setting up environment variables and running commands from the command line in the OculusSite projects architecture.                                                    |
| [Procfile](https://github.com/kashishvjain/Oculus-2022-be/blob/master/Procfile)   | Enables web server deployment by defining the command to run the server on a specified port. Essential for launching the project within the specified architecture of the Oculus-2022-be repository. |
| [Pipfile](https://github.com/kashishvjain/Oculus-2022-be/blob/master/Pipfile)     | Defines dependencies for Django, Django REST framework, Firebase, and more in the Pipfile. Supports web development for Oculus-2022-be repository.                                                   |

</details>

<details closed><summary>OculusSite</summary>

| File                                                                                                       | Summary                                                                                                                                                                                                                                                                                                      |
| ---                                                                                                        | ---                                                                                                                                                                                                                                                                                                          |
| [wsgi.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/OculusSite/wsgi.py)                   | Exposes WSGI callable for OculusSite project. Sets DJANGO_SETTINGS_MODULE and retrieves WSGI application using Django core. Supports Django deployment.                                                                                                                                                      |
| [asgi.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/OculusSite/asgi.py)                   | Exposes ASGI callable for the OculusSite project, setting DJANGO_SETTINGS_MODULE dynamically. Aligns with the parent repositorys architecture by enabling asynchronous server applications.                                                                                                                  |
| [credentials.json](https://github.com/kashishvjain/Oculus-2022-be/blob/master/OculusSite/credentials.json) | Exposes Firebase service account credentials for authentication in the Oculus-2022-be repositorys backend architecture.                                                                                                                                                                                      |
| [urls.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/OculusSite/urls.py)                   | Routes URLs to views by configuring OculusSite URLs. Includes admin URLs and links to APIserver URLs for web application navigation.                                                                                                                                                                         |
| [settings.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/OculusSite/settings.py)           | Defines Django settings for OculusSite project, including secret key, debug status, installed apps, CORS configuration, middleware, database setup, password validators, internationalization settings, and static file handling. It integrates with Django 3.2.8 and utilizes django-heroku for deployment. |

</details>

<details closed><summary>APIserver</summary>

| File                                                                                                      | Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---                                                                                                       | ---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| [apps.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/apps.py)                   | Defines the configuration for the APIserver app within the Oculus-2022-be repository, specifying the default auto field type and the app name. This file helps manage settings and behavior specific to the APIserver component.                                                                                                                                                                                                                                                                               |
| [models.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/models.py)               | Defines Django models for the APIserver to interact with the database. Maps data structure for the applications backend functionality within the Oculus-2022-be repository.                                                                                                                                                                                                                                                                                                                                    |
| [credentials.json](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/credentials.json) | Validates and stores sensitive API credentials for the Oculus-2022-be API server. Essential for securely managing external service integrations within the repository architecture.                                                                                                                                                                                                                                                                                                                            |
| [urls.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/urls.py)                   | Defines URL patterns for various API endpoints for data management and notifications. Supports registration, team updates, event details retrieval, chat, payment status, and notifications. Introduces dynamic event identifier and CSV download feature for improved functionality.                                                                                                                                                                                                                          |
| [admin.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/admin.py)                 | Registers models with the Django admin interface in the `admin.py` file under the `APIserver` directory. It plays a crucial role in managing and organizing data models within the Oculus-2022-be repository architecture.                                                                                                                                                                                                                                                                                     |
| [tests.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/tests.py)                 | Verifies APIserver functionality by creating test cases using Djangos test framework.                                                                                                                                                                                                                                                                                                                                                                                                                          |
| [views.py](https://github.com/kashishvjain/Oculus-2022-be/blob/master/APIserver/views.py)                 | The `views.py` file in the `APIserver` module of the repository serves as a crucial component in handling views and responses for the API endpoints. It leverages Django and Firebase Admin libraries to interact with the database and manage file uploads securely. This file plays a significant role in orchestrating the communication between the front-end and the backend system of the Oculus application, ensuring seamless user interactions and data processing within the platforms architecture. |

</details>

---

##  Getting Started

**System Requirements:**

* **Python**: `version x.y.z`

###  Installation

<h4>From <code>source</code></h4>

> 1. Clone the Oculus-2022-be repository:
>
> ```console
> $ git clone https://github.com/kashishvjain/Oculus-2022-be
> ```
>
> 2. Change to the project directory:
> ```console
> $ cd Oculus-2022-be
> ```
>
> 3. Install the dependencies:
> ```console
> $ pip install -r requirements.txt
> ```

###  Usage

<h4>From <code>source</code></h4>

> Run Oculus-2022-be using the command below:
> ```console
> $ python manage.py runserver
> ```

---

