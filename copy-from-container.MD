## Copy from container
```docker cp <container>:<src-path> <local-dest-path>``` 
#### Example
```docker cp 5d49c9f868a5:/techniques-all-dbs.sql ./backups ``` 

## Copy to container
```docker cp <src-path> <container>:<dest-path>```
#### Example
```docker cp techniques-all-dbs.sql 5d49c9f868a5:. ```
