---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3Scale Account Management API End User Change Plan
  description: End user change plan.
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/api/accounts/{account_id}/applications/{id}/change_plan.xml:
    put:
      summary: Application Change Plan
      description: Application change plan.
      operationId: application
      x-api-path-slug: adminapiaccountsaccount-idapplicationsidchange-plan-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the application
      - in: query
        name: plan_id
        description: id of the new application plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Change
      - Plan
  /admin/api/accounts/{account_id}/users/{id}/admin.xml:
    put:
      summary: User change Role to Admin
      description: User change role to admin.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidadmin-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Change
      - Role
      - To
      - Admin
  /admin/api/accounts/{account_id}/users/{id}/member.xml:
    put:
      summary: User change Role to Member
      description: User change role to member.
      operationId: user
      x-api-path-slug: adminapiaccountsaccount-idusersidmember-xml-put
      parameters:
      - in: path
        name: account_id
        description: id of the account
      - in: path
        name: id
        description: id of the user
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - User
      - Change
      - Role
      - To
      - Member
  /admin/api/accounts/{id}/change_plan.xml:
    put:
      summary: Account Change Plan
      description: Account change plan.
      operationId: account
      x-api-path-slug: adminapiaccountsidchange-plan-xml-put
      parameters:
      - in: path
        name: id
        description: id of the account
      - in: query
        name: plan_id
        description: id of the target account plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      responses:
        200:
          description: OK
      tags:
      - Account
      - Change
      - Plan
  /admin/api/services/{service_id}/end_users/{username}/change_plan.xml:
    put:
      summary: End User Change Plan
      description: End user change plan.
      operationId: end_user
      x-api-path-slug: adminapiservicesservice-idend-usersusernamechange-plan-xml-put
      parameters:
      - in: query
        name: plan_id
        description: id of the new end user plan
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: path
        name: service_id
        description: id of the service
      - in: path
        name: username
        description: username (unique identifier) of the end user
      responses:
        200:
          description: OK
      tags:
      - End
      - User
      - Change
      - Plan
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