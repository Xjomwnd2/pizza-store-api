# pizza-store-api
Build .NET Applications with C#
# Create README.md
cat > README.md << 'EOF'
# Pizza Store API

ASP.NET Core Web API for managing a pizza store - W01 Assignment

## Description
RESTful Web API that supports CRUD operations for pizza management.

## Technologies
- ASP.NET Core 8.0
- C#
- Web API Controllers

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /pizza | Get all pizzas |
| GET | /pizza/{id} | Get pizza by ID |
| POST | /pizza | Create new pizza |
| PUT | /pizza/{id} | Update pizza |
| DELETE | /pizza/{id} | Delete pizza |

## Running the API
```bash
dotnet restore
dotnet run
```

The API will be available at: `http://localhost:5000`

## Testing the API

### Get all pizzas
```bash
curl -X GET http://localhost:5000/pizza
```

### Create a pizza
```bash
curl -X POST http://localhost:5000/pizza \
  -H "Content-Type: application/json" \
  -d '{"name":"Hawaiian Paradise","isGlutenFree":false}'
```

## Assignment Requirements Met
- ✅ Completed Microsoft Learn module
- ✅ Implemented full CRUD operations
- ✅ Added additional pizza record
- ✅ Tested all endpoints

## Author
[Your Name] - W01 Assignment
EOF

# Add and commit README
git add README.md
git commit -m "Add README with API documentation"
git push