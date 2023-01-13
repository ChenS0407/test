# Get build node information (extension interface)

### Request method/request path

#### GET /ms/openapi/api/apigw/v3/environment/projects/{projectId}/nodes/extListNodes

### Resource description

#### Get build node information (extension interface)

### Input parameter description

#### Path parameter

| Parameter name | Parameter type | must | Parameter description | Default value |
| :------------- | :------------- | :--- | :-------------------- | :------------ |
| projectId      | string         | yes  | Item ID               |               |

#### response

| HTTP code | description          | Parameter type                                               |
| :-------- | :------------------- | :----------------------------------------------------------- |
| 200       | successful operation | Data return wrapper model List Node Information (permissions) |

#### Request sample

```
curl -X GET '[Please replace API address bar request address]' 
```

#### HEADER example

```
accept: application/json Content-Type: application/json 
```

### Return example -200

```
curl -X GET '[API URL]?debug={debug}&amp;num={num}&amp;fromStart={fromStart}&amp;start={start}&amp;end={end}&amp;tag={tag}&amp;jobId={jobId}&amp;executeCount={executeCount}' \
-H 'X-DEVOPS-UID:xxx'
```

## Data return wrapper model List Node Information (permissions)

| Parameter name | Parameter type                        | must | Parameter description |
| :------------- | :------------------------------------ | :--- | :-------------------- |
| data           | List< Node information (permissions)> | no   | data                  |
| message        | string                                | no   | Error message         |
| status         | integer                               | is   | Status code           |

## Node information (permission)

| Parameter name   | Parameter type | must | Parameter description                                        |
| :--------------- | :------------- | :--- | :----------------------------------------------------------- |
| pipelineRefCount | integer        | no   | Number of pipeline Job references                            |
| nodeHashId       | string         | is   | Environmental HashId                                         |
| displayName      | string         | no   | Display name                                                 |
| ip               | string         | is   | IP                                                           |
| canEdit          | boolean        | no   | Whether it can be edited                                     |
| nodeStatus       | string         | is   | Node state                                                   |
| nodeType         | string         | is   | Node type                                                    |
| osName           | string         | no   | Operating system                                             |
| agentStatus      | boolean        | is   | agent state                                                  |
| operator         | string         | no   | Responsible person                                           |
| canUse           | boolean        | no   | Whether it can be used                                       |
| bakOperator      | string         | no   | Backup owner                                                 |
| lastBuildTime    | string         | no   | Number of pipeline Job references                            |
| lastModifyUser   | string         | no   | Last modifier                                                |
| createTime       | string         | no   | Creation/import time                                         |
| lastModifyTime   | string         | no   | Last revision time                                           |
| name             | string         | is   | Node name                                                    |
| bizId            | integer        | no   | Owning service. The default value -1 indicates that no service is bound |
| canDelete        | boolean        | no   | Whether it can be deleted                                    |
| nodeId           | string         | is   | Node Id                                                      |
| createdUser      | string         | is   | founder                                                      |
| gateway          | string         | no   | Gateway area                                                 |
| agentHashId      | string         | no   | agent hash id                                                |
