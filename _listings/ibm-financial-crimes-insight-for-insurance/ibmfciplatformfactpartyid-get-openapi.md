---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Retrieve party data from the
    database, for the id
  description: This method is used to retrieve party data from the database
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/entity/relatedparties/{systemId}/{remoteReference}:
    get:
      summary: This method is used to retrieve the set of explicitly related parties
        and implicitly related entities for the supplied externally sourced reference
        party
      description: |-
        A data source must be configured in the appropriate server.xml to use ISII. Ensure that the following has been included:

        &lt;dataSource beginTranForResultSetScrollingAPIs="false" id="ISIIDB" isolationLevel="TRANSACTION_READ_COMMITTED" jndiName="jdbc/isii"&gt;

        &lt;jdbcDriver javax.sql.DataSource="com.ibm.db2.jcc.DB2XADataSource" libraryRef="DB2_LIB"/&gt;

        &lt;properties.db2.jcc databaseName="ISII" password="${isii_db_pass}" portNumber="${isii_db_port}" serverName="${isii_host}" user="${isii_db_user}"/&gt;

        &lt;connectionManager connectionTimeout="60s" maxIdleTime="3m" maxPoolSize="200" minPoolSize="0"/&gt;

        &lt;/dataSource&gt;

        Where password, portNumber, serverName, and user values are replaced with the appropriate properties or environment variables for your configuration.
      operationId: getRelatedObjects
      x-api-path-slug: ibmfciplatformfactentityrelatedpartiessystemidremotereference-get
      parameters:
      - in: query
        name: minRelatedScore
        description: Minimum matching score for implicit relationships
      - in: path
        name: remoteReference
        description: Remote reference object key
      - in: path
        name: systemId
        description: Remote reference system ID
      responses:
        200:
          description: OK
      tags:
      - This
      - Method
      - Is
      - Used
      - To
      - Retrieve
      - Set
      - Of
      - Explicitly
      - Related
      - Parties
      - Implicitly
      - Related
      - Entitiesthe
      - Supplied
      - Externally
      - Sourced
      - Reference
      - Party
  /ibm/fci/platform/fact/party:
    put:
      summary: Insert party data into the database
      description: This method is used to insert party data into the database.  The
        XML schema is defined in the PARTY.XSD file.
      operationId: putParty
      x-api-path-slug: ibmfciplatformfactparty-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Party
      - Data
      - Into
      - Database
  /ibm/fci/platform/fact/party/{id}:
    get:
      summary: Retrieve party data from the database, for the id
      description: This method is used to retrieve party data from the database
      operationId: getParty
      x-api-path-slug: ibmfciplatformfactpartyid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Party
      - Data
      - From
      - Database
      - The
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---