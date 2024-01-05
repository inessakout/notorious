[service-notorious](../../README.md) / [API](../README.md) / [How to use](./README.md) / Pagination

# Pagination

Results of requests with list have a pagination system. The page number can be selected with the
query field `page`. The reponse's body `pagination` property give information about the total number
of pages, the number of elements by pages and the current page. 

## Example

```
GET /projects?page=3
```
