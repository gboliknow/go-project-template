

````markdown
# Go Project Template

A clean and minimal starter template for new Go projects. This template provides a well-structured layout you can use as a foundation for your applications.

## 🚀 Usage

1. **Create a new project from this template**  
   Click **"Use this template"** on GitHub, or run with GitHub CLI:  
   ```bash
   gh repo create my-new-project --template=gboliknow/go-project-template
````

2. **Initialize your Go module**

   ```bash
   cd my-new-project
   go mod init github.com/username/my-new-project
   go mod tidy
   ```

3. **Run the project**

   ```bash
   go run ./cmd/app
   ```

## 📂 Project Structure

```
cmd/            # Application entry points (main.go lives here)
internal/       # Private application code (business logic, handlers, etc.)
pkg/            # Public reusable libraries (optional)
api/            # API definitions (OpenAPI, gRPC, etc.)
configs/        # Configuration files
docs/           # Documentation
scripts/        # Helper scripts (migrations, CI/CD, etc.)
test/           # Integration/e2e tests
```

## ✅ Notes

* Keep `main.go` minimal (only wiring and bootstrapping).
* Place tests next to the code (`*_test.go`) or inside `test/` for integration tests.
* Use `pkg/` only for code you expect to reuse across multiple projects.
* `internal/` is for application-specific code and cannot be imported by other modules.

## 📌 Next Steps

* Add dependencies as needed with `go get`
* Set up logging, routing, or database integration depending on your project
* Start coding your business logic inside `internal/`


