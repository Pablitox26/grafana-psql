# Quick Starter

1. Clone the repository

2. Clone the file ```.env.template``` and rename the copy to ```.env```

3. Fill the environment variables defined in the ```.env```

4. Clone the file ```.env.db.template``` and rename the copy to ```.env.db```

5. Fill the environment variables defined in the ```.env.db```

6. Execute: 
```
docker-compose up -d
```

## Query example

```sql
SELECT 
  created_at as "time",
  "tempAmbient" 
FROM habitacion
WHERE 
  $__timeFilter(created_at)
ORDER BY created_at
```

## Stack used
* MongoDB
* Grafana