👨‍💻 **SuperHeroService (SuperHero Service):**
   - 🔄 The `SuperHeroService` class implements the `ISuperHeroService` interface and represents the service layer responsible for processing superhero data.
   - 🏗️ Through the constructor, it acquires an instance of the `DataContext` providing access to a database using Entity Framework Core.
   - ➕ `AddHero`: Adds a new superhero, updates the database, and returns the updated list of all heroes.
   - ➖ `DeleteHero`: Deletes a superhero with a specific ID, updates the database, and returns the updated list. Returns `null` if the hero is not found.
   - 📋 `GetAllHeroes`: Lists all superheroes.
   - 🎯 `GetSingleHero`: Retrieves a superhero with a specific ID. Returns `null` if the hero is not found.
   - 🔄 `UpdateHero`: Updates a superhero with a specific ID, updates the database, and returns the updated list. Returns `null` if the hero is not found.

🎮 **SuperHeroController (SuperHero Controller):**
   - 🔄 The `SuperHeroController` class is used to handle HTTP requests and directs operations through the `SuperHeroService`.
   - 🔄 Through the constructor, it injects the dependency of `ISuperHeroService`.
   - 📋 `GetAllHeroes`: Handles the HTTP GET request to retrieve all superheroes.
   - 🎯 `GetSingleHero`: Handles the HTTP GET request to retrieve a superhero with a specific ID. Returns 404 Not Found if the hero is not found.
   - ➕ `AddHero`: Handles the HTTP POST request to add a new superhero.
   - 🔄 `UpdateHero`: Handles the HTTP PUT request to update a superhero with a specific ID. Returns 404 Not Found if the hero is not found.
   - ➖ `DeleteHero`: Handles the HTTP DELETE request to delete a superhero with a specific ID. Returns 404 Not Found if the hero is not found.
