## `library.localhost:8000`

### Create new app
```
bench new-app library_management
```

### get existing app
```
bench get-app crm
```

### Create `library.localhost` site
```
bench new-site library.localhost
```

### add sites to add-to-hosts
```
bench --site library.localhost add-to-hosts
```

### Install app in sites
```
bench --site library.localhost install-app 
library_management
```

### Shell
```
bench --site library.localhost console
```

### DB Shell
```
bench --site library.localhost mariadb
```

### Backup database
```
bench --site library.localhost backup
```

## Enable Developer mode
```
bench set-config -g developer_mode true
```

# Start

```
bench start
```

### See table description after create DocType

```
bench --site library.localhost mariadb

# then

desc tabArticle;

```

### enable server_script_enable
```
bench set-config -g server_script_enabled true
```