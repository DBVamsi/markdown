### Retrieve an album
Retrieves the data of specific album

`GET https://yourcompany.com/api/v1/album/{album_id}`

where {album_id} is the unique id of the album to be retrieved.

---
### Retrieve all albums
Retrieves all available albums if no album_id is specified

`GET https://yourcompany.com/api/v1/album`

---
### Create an album
Creates an album with an unique album_id.

`POST https://yourcompany.com/api/v1/album`

```
{
  body
}
```
where {body} is used for creation parameters.

---
### Update an album
Updates an existing album.

`PUT https://yourcompany.com/api/v1/album/{album_id}`
```
{
body
}
```
where {album_id} is unique id of the album to be updated. {body} is the update parameters.

---
### Delete an album
Deletes an existing album.

`DELETE https://yourcompany.com/api/v1/album/{album_id}`

where {album_id} is the unique id of the album to be deleted.

---
### Print an album
Prints out an album.

`POST https://yourcompany.com/api/v1/album/{album_id}/print`

where {album_id} is the unique id of the album to be printed.

---
---

Click [here](https://dbvamsi.github.io/markdown/) to get back to index.
