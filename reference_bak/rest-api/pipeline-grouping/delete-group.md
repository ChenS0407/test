# 删除分组

### 请求方法/请求路径

#### DELETE  /ms/openapi/api/apigw/v3/projects/{projectId}/pipelineGroups/groups/{groupId}

### 资源描述

#### 删除分组

### 输入参数说明

#### Path参数

| 参数名称 | 参数类型 | 必须 | 参数说明 | 默认值 |
| :--- | :--- | :--- | :--- | :--- |
| groupId | string | 是 | 分组ID |  |

#### 响应

| HTTP代码 | 说明 | 参数类型 |
| :--- | :--- | :--- |
| 200 | successful operation | [数据返回包装模型Boolean](delete-group.md) |

#### 请求样例

```javascript
curl -X DELETE '[请替换为API地址栏请求地址]'
```

#### HEADER样例

```javascript
accept: application/json
Content-Type: application/json
```

### 返回样例-200

```javascript
{
  "data" : true,
  "message" : "String",
  "status" : 0
}
```

## 数据返回包装模型Boolean

| 参数名称 | 参数类型 | 必须 | 参数说明 |
| :--- | :--- | :--- | :--- |
| data | boolean | 否 | 数据 |
| message | string | 否 | 错误信息 |
| status | integer | 是 | 状态码 |
