---
sidebar_position: 3
---

# Configuration Parameters

| Sl# | Parameter Name             | Description                                                                                     | Allowed Values/Examples                                                                                                                       |
|-----|----------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|
| 1.  | ALLOW_SAFE_DELETE          | Allow deletion of table rows without a filter criteria.                                         | <ul><li>true(default)</li><li>false</li></ul>                                                                                                 |
| 2.  | DB_ID                      | Logical Identifier of the database to be used in API URL. This is not the name of the database. | <ul><li>db(default)</li></ul>                                                                                                                 |
| 3.  | DB_URL                     | Database connection URL in JDBC format.                                                         | <ul><li> jdbc:mysql://DB_SERVER_HOST:DB_PORT/DB_NAME (MySQL)</li><li> jdbc:postgresql://DB_SERVER_HOST:DB_PORT/DB_NAME (PostgreSQL)</li></ul> |
| 4.  | DB_USER                    | Database user name                                                                              | -                                                                                                                                             |
| 5.  | DB_PASSWORD                | Database password                                                                               | -                                                                                                                                             |
| 6.  | SERVER_PORT                | Webserver PORT                                                                                  | <ul><li>8080(default)</li></ul>                                                                                                               |
| 7.  | GZIP_ENABLED               | Whether response compression is enabled                                                         | <ul><li>true</li><li>false (default)</li></ul>                                                                                                |
| 8.  | GZIP_MIN_RESPONSE_SIZE     | Minimum "Content-Length" value in KB that is required for compression to be performed.          | <ul><li>1024(default)</li></ul>                                                                                                               |
| 9.  | ENABLE_DATETIME_FORMATTING | Whether to enable date time formatting in response.                                             | <ul><li>false(default)</li><li>true</li></ul>                                                                                                 |
| 10. | TIME_FORMAT                | Time format                                                                                     | <ul><li>`HH:mm:ss`(default)</li></ul>                                                                                                         |
| 11. | DATE_FORMAT                | Date format                                                                                     | <ul><li>`yyyy-MM-dd`(default)</li></ul>                                                                                                       |
| 12. | DATE_TIME_FORMAT           | Date time format                                                                                | <ul><li>`yyyy-MM-dd HH:mm:ss`(default)</li></ul>                                                                                              |
| 13. | ENABLE_AUTH                | Enable authentication and authorization                                                         | <ul><li>`false`(default)</li><li>`true`</li></ul>                                                                                             |
| 14. | AUTH_DATA_SOURCE           | Provide the absolute path of the auth data as a file.                                           | -                                                                                                                                             |
| 15. | DEFAULT_FETCH_LIMIT        | Limits the number of rows that will be retrieved for a read query.                              | 100                                                                                                                                           |
| 16. | PROMETHEUS_EXPORT_ENABLED  | Enable Monitoring with Prometheus and Grafana Observability Stack                               | <ul><li>false(default)</li><li>true</li></ul>                                                                                                 |
| 17. | DATADOG_EXPORT_ENABLED     | Enable Monitoring with Datadog                                                                  | <ul><li>false(default)</li><li>true</li></ul>                                                                                                 |
| 18. | DATADOG_API_KEY            | Datadog API Key                                                                                 | -                                                                                                                                             |
| 19. | DATADOG_APPLICATION_KEY    | Datadog Application Key                                                                         | -                                                                                                                                             |
| 20. | DATADOG_EXPORT_URI         | Datadog export URI - this is where the data will be posted.                                     | -                                                                                                                                             |    
| 21. | DATADOG_EXPORT_INTERVAL    | Interval after which the data will be scraped and posted.                                       | Default: 30s                                                                                                                                  |  
| 22. | INCLUDED_SCHEMAS           | Comma separated list of schemas from which the meta-data about tables will be loaded.           | -                                                                                                                                             |  
| 23. | CORS_ORIGIN_URL           | Comma seperated list of allowed Cross Origin URLs from where requests will be sent to server.           | Default: *                                                                                                                                             |  
| 24. | CORS_HEADERS_ALLOWED           | Comma seperated list of Headers which will be allowed for the requests.           | Default: *                                                                                                                                             | 
| 25. | CORS_METHODS_ALLOWED           | Comma seperated list of Methods which will be allowed for the requests.           | Default: `GET,POST`                                                                                                                                             | 



:::tip

If DB2Rest is connected to [multiple databases](./multidb/connect-multiple-db) do not use configurations 2-5. 
Follow the guide for connecting to [multiple databases](./multidb/connect-multiple-db).

:::


:::info

Date time format parameter is only applicable for output / response. 

:::


:::warning

In case request attributes, only ISO data-time formats are supported. 

:::
