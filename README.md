```bash
# 1. Generate Application Key (sets encryption key in .env)
php artisan key:generate

# 2. Start Local Development Server (runs the app locally)
php artisan serve

# 3. Create Storage Link (makes storage files publicly accessible)
php artisan storage:link

# 4. Create a Model (creates the Eloquent model class)
php artisan make:model Product

# 5. Create Controllers (standard vs CRUD resource controller)
php artisan make:controller ProductController
php artisan make:controller ProductController --resource

# 6. Create a Migration (creates table schema file)
php artisan make:migration create_products_table

# 7. Create a Seeder (populates database with sample records)
php artisan make:seeder ProductSeeder

# 8. Create a Factory (generates fake test data)
php artisan make:factory ProductFactory --model=Product

# 9. List Commands & Routes (views all available CLI tasks or routes)
php artisan list
php artisan route:list

# 10. Database Migrations (run, rollback, refresh, and seed)
php artisan migrate               # Run pending migrations
php artisan migrate:rollback      # Roll back last batch
php artisan migrate:refresh       # Reset and re-run all migrations
php artisan migrate --seed        # Run migrations and seed data

# Shortcut: create Model, Migration, Factory, Seeder & Controller all in one
php artisan make:model Product -a