Project Name: Data Dashboard App

Tagline: A python application that aggregates and presents data in an interactive dashboard.

Team:

Adama Dolo : the only one to do all the tasks

Technologies:

Libraries: Pandas, NumPy, Matplotlib
Languages: Python
Platforms: Flask, Dash
Frameworks: Bootstrap
Hardware: None
Books: "Python Data Science Handbook" by Jake VanderPlas
Resources: "Flask Web Development with Python Tutorial" by Corey Schafer
Platforms:
Flask: Flask is a micro web framework written in Python. It is lightweight and easy to use. Flask allows for the development of small to medium-sized web applications, and is well-suited for prototyping and small-scale deployment.
Django: Django is a high-level web framework written in Python. It is more powerful and feature-rich than Flask. Django is well-suited for large-scale web applications, and is often used for enterprise-level projects.
The final decision was to use Flask as it was more lightweight and easier to use. It also allowed for a faster development time and was more suitable for our small-scale web application.

Frameworks:
Bootstrap: Bootstrap is a popular front-end framework that provides a consistent look and feel for web applications. It is easy to use and requires minimal customization. Bootstrap also provides a responsive design, making it suitable for use on various devices.
Foundation: Foundation is another popular front-end framework. It is similar to Bootstrap but offers more advanced features such as more customization options and more control over the layout.
The final decision was to use Bootstrap as it was more widely used and had more resources and tutorials available. The responsive design also made it more suitable for our project as it needed to work on various devices.

Challenges:

The problem the Portfolio Project is intended to solve is the lack of a centralized platform for industrial companies to view and analyze their data. Many companies have data scattered across multiple systems and platforms, making it difficult to gain insights and make informed decisions. The project aims to aggregate this data and present it in an interactive dashboard, providing users with a clear and comprehensive view of their data.

The Portfolio Project will not solve the underlying issues that may be causing the scattered data, such as lack of proper data management systems. It is intended to serve as a tool for data visualization and analysis, not data management.

The Portfolio Project will help industrial companies and their employees, particularly those in data analysis and decision-making roles. Users will include data analysts, managers, and executives who need access to the data and insights in order to make informed decisions.

The project is not dependent on a specific locale as it can be used by industrial companies from any location. The data used in the app can be from any source as long as it can be integrated and presented in the app.

Risks:

Technical Risks:

Data integration: One of the technical risks is the challenge of integrating data from multiple sources and systems into the app. If data cannot be properly integrated, the app may not provide accurate or comprehensive insights. The potential impact is that the app may not be useful to the users and the project may fail. To mitigate this risk, we will thoroughly test data integration during the development process and have a plan in place for handling any data compatibility issues that arise.
Scalability: Another technical risk is the app's ability to handle large amounts of data and handle traffic from multiple users. The potential impact is that the app may become slow or unresponsive, leading to a poor user experience. To mitigate this risk, we will design the app with scalability in mind and have a plan for adding more resources and infrastructure as needed.
Non-technical Risks:

Adoption: One of the non-technical risks is the challenge of getting industrial companies to adopt and use the app. The potential impact is that the project may not be successful and may not have a positive return on investment. To prevent this negative outcome, we will conduct market research to understand the needs of industrial companies and tailor the app to their specific needs. We will also reach out to potential users and gather feedback during the development process to ensure that the app meets their needs.
Data security: Another non-technical risk is the protection of sensitive data that may be stored in the app. The potential impact is that the app may become a target for cyber-attacks, leading to loss of data or damage to the company's reputation. To prevent this negative outcome, we will ensure that all data is stored securely, and that appropriate security measures are in place to protect against unauthorized access or breaches.

Infrastructure:

Branching and Merging: Our team will use the GitHub flow for branching and merging. This involves creating a new branch for each feature or bug fix and merging it back into the master branch after it has been reviewed and approved by at least one other team member. This strategy ensures that the master branch always contains stable and tested code.

Deployment: Our strategy for deployment is to use continuous integration and continuous deployment (CI/CD) to automatically deploy the app to a staging environment for testing and then to a production environment after it has been thoroughly tested. This allows us to quickly and easily deploy new features and updates to the app.

Data Population: We will use scripts to extract and transform the data from various sources and then use APIs to load the data into the app. This will automate the process of data population and ensure that the data is accurate and up to date.

Testing: We will use a combination of manual testing and automated testing to ensure the app is functioning correctly. For manual testing, our team will use test cases to test different scenarios and ensure that the app meets our requirements. For automated testing, we will use tools such as Selenium and Pytest to write unit tests and integration tests. We will also use tools such as Travis CI to automatically run tests on each code change. This will help us catch any bugs or issues early in the development process and ensure that the app is thoroughly tested before deployment.

Existing Solutions:

Tableau
Power BI
Looker
QlikView
SAP Lumira
Similarities:

All of the above solutions are data visualization and analysis tools that provide interactive dashboards for data exploration.
They all offer the ability to connect to a wide variety of data sources and provide data visualization options such as charts, graphs, and tables.
They all provide data exploration and analysis capabilities, allowing users to filter, group, and aggregate data to gain insights.
Differences:

Tableau is a more advanced tool with a larger feature set, including advanced data visualization options and data blending capabilities. Power BI and Looker are more limited in terms of features and functionality, but are more affordable.
QlikView and SAP Lumira are more focused on enterprise-level solutions, while Tableau and Power BI are more geared towards small and medium-sized businesses.
The choice to use Transform coding as an image compression algorithm is based on its ability to achieve high compression ratios without losing too much image quality. Transform coding is a class of image compression techniques that utilize mathematical transforms, such as the Discrete Cosine Transform (DCT), to represent the image data in a more compact form. There are other classes of image compression techniques such as lossless compression and fractal compression, but Transform coding is a better fit for our needs as it allows for a good balance of compression ratio and image quality.



Architecture




APIs and Methods

API Routes for Web Client Communication:

/login: Allows users to log in to the application with their credentials.
/logout: Allows users to log out of the application.
/data: Returns the processed data in JSON format for the visualization layer.
/dashboard: Renders the dashboard visualization in HTML.
/settings: Allows users to update their account settings.
/admin: Allows admin users to manage the data sources and processing settings for the application.

API Endpoints for Other Clients:

/api/data: Returns the processed data in JSON format for external clients to consume.
/api/sources: Returns a list of available data sources for external clients to use.
/api/documentation: Provides documentation on how to use the API endpoints.

3rd Party APIs:

Google Analytics API: Allows the application to retrieve and process data from Google Analytics.
Twitter API: Allows the application to retrieve and process data from Twitter.
Facebook API: Allows the application to retrieve and process data from Facebook.
It's important to note that the specific API routes, endpoints, and 3rd party APIs will depend on the specific requirements and design of the application.

Data Model





User Stories

User stories are a way to describe the desired functionality of a software system from the perspective of the end user. They are used in Agile development methodologies as a way to capture requirements and organize work.

A user story should be written in a simple and concise format, typically in the following format:

As a [user], I want [functionality], so that [benefit].

Some examples of user stories include:

As a dashboard administrator, I want to be able to add new data sources, so that I can easily update the data displayed on the dashboard.
As a dashboard user, I want to be able to filter the data displayed on the dashboard, so that I can easily find the information I need.
As a dashboard user, I want to be able to export the data displayed on the dashboard to a CSV file, so that I can analyze the data in a spreadsheet program.
When creating user stories, it is important to avoid making them too general. This can happen when the user story does not clearly define the user, functionality, or benefit, or when the user story is too broad and encompasses multiple functionality.

Here are some examples of user stories that are too general:

As a user, I want to be able to interact with the dashboard, without specifying what kind of interaction is needed.
As a user, I want the dashboard to be easy to use, without specifying what makes it easy to use.
As a user, I want to be able to customize the dashboard, without specifying what is meant by customization.
In the "User Stories" section of your MVP, you can define 3-5 detailed user stories that will be satisfied when your MVP is complete:

As a dashboard user, I want to be able to select different data sources to view on the dashboard, so that I can easily compare data from different sources.
As a dashboard administrator, I want to be able to set permissions for different users, so that I can control who can access and edit the data on the dashboard.
As a dashboard user, I want to be able to create and customize widgets, so that I can display the data in a way that is most useful to me.
As a dashboard user, I want to be able to export the data displayed on the dashboard to a CSV file, so that I can analyze the data in a spreadsheet program.
As a dashboard user, I want to be able to filter the data displayed on the dashboard, so that I can easily find the information I need.
It's important to note that these are just examples and you should adapt them to your specific use case.



