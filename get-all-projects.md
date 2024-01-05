[service-notorious](../../README.md) / [API](../README.md) / [Projects](./README.md) / Get all projects

# Get all projects

Returns all projects.

```
GET /projects
```

## Query fields

| Name           | Description                                          |
|:---------------|:-----------------------------------------------------|
| `workspace-id` | Returns only the projects related to this workspace. |

## Example

```
GET /projects?workspace-id=5
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
  "projects": [{
    "id": 1,
    "workspace_id": 5,
    "title": "A title",
    "query": "cat",
    "language": "fr",
    "page": "https://www.cat.com",
    "created_at": "2022-11-30 10:10:10",
    "email": "bobi@mail.fr",
    "is_done": true,
    "is_finish": true,
    "is_all_recup": true,
    "fame": 2345
  }, {
    "id": 2,
    "workspace_id": 5,
    "title": "A new Title",
    "query": "cat",
    "language": "fr",
    "page": "https://www.cat.com",
    "created_at": "2022-11-30 10:10:10",
    "email": "bobi@mail.fr",
    "is_done": true,
    "is_finish": true,
    "is_all_recup": true,
    "fame": 2345
  }],
  "pagination": {
    "current_page": 1,
    "total_page": 5,
    "limit": 20
  }
}
```
