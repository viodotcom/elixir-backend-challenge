# Backend Coding Challenge

## Geolocation Service

### Overview

You are tasked with developing a geolocation service that processes raw geolocation data from a CSV file (`data_dump.csv`) and exposes it via a REST API. 

Sample data:

```
ip_address,country_code,country,city,latitude,longitude,mystery_value
200.106.141.15,SI,Nepal,DuBuquemouth,-84.87503094689836,7.206435933364332,7823011346
160.103.7.140,CZ,Nicaragua,New Neva,-68.31023296602508,-37.62435199624531,7301823115
70.95.73.73,TL,Saudi Arabia,Gradymouth,-49.16675918861615,-86.05920084416894,2559997162
,PY,Falkland Islands (Malvinas),,75.41685191518815,-144.6943217219469,0
125.159.20.54,LI,Guyana,Port Karson,-78.2274228596799,-163.26218895343357,1337885276
```

### Requirements

1. **Develop a Library/Component** with two main features:
    - A service that parses the CSV file, sanitizes the data, and persists it in a database.
    - An interface to provide programmatic access to the geolocation data.
2. **Develop a REST API** that uses the library to expose the geolocation data, with at least one endpoint: `GET /api/geolocation/<ip_address>` to return location details.
3. **Testing**: Include unit and/or integration tests covering at least 80% of the code, with a coverage report.
4. **Error Handling and Logging**: Implement graceful error handling for import failures, invalid API requests, and deployment issues. Include basic logging for import statistics and API requests.
5. **Deployment**: Deploy the project on a cloud platform of your choice (e.g., Heroku, Fly.io, Digital Ocean, AWS, Google Cloud, Azure). Import all the data or part of it according to the cloud platform quota limits.
6. **Documentation:** Provide a README file to document the project and your choices.

### Notes

- **Time Estimate**: Allocate 4-8 hours, prioritizing quality over completeness.
- **Tech Stack Choice**: Any of Ruby, Elixir, Python, or Golang is permitted. Frameworks are allowed.
- **Data**: The CSV contents are fake; no need to verify real-world data accuracy.
- **Local Development**: Use a database container (e.g., PostgreSQL, MySQL) in Docker for local testing.
- **AI Usage**: If AI tools are used, disclose their role transparently in the [`README.md`](http://README.md) for the project.

### Sharing the solution

1. Create one or more repos on **GitHub** and add `@zekus` `@prodis` `@rinaldifonseca`as collaborators.
2. Follow the instructions in the email

### Follow-Up Interview

Please be prepared for a 60-90 minute discussion and live coding session, during which you will be asked to **share your screen and record the session** to ensure a fair and objective evaluation.

- Walk through your code and explain key components, decisions, and trade-offs.
- Make live modifications.
- Discuss hypothetical scenarios.
- Answer questions on trade-offs and alternative approaches.

**Please ensure that your development environment is functioning properly and that your application runs smoothly for the technical interview.**
