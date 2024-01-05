[service-notorious](../../README.md) / [API](../README.md) / [Projects](./README.md) / Get a project

# Get a project

Get a project by id.

```
GET /projects/:id
```

## Parameters

| Name | Description        |
|------|--------------------|
| `id` | ID of the project. |

## Example

```
GET /projects/3
```

```json
{
  "user": {
    "id": 1,
    "workspaces": [5],
    "role": "customer"
  }
}
```

Response

```
200 OK
```

```json
{
  "id": 3,
  "workspace_id": 5,
  "title": "A title",
  "query": "cat",
  "language": "fr",
  "page": "https://www.cat.com",
  "created_at": "2022-11-30 10:10:10",
  "email": "bobi@mail.fr",
  "is_done": true,
  "is_finish": true,
  "is_all_recup": true
}
```
