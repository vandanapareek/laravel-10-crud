# Laravel 10 crud

We will create a product crud application using laravel 10. we will create a products table with name and detail columns using laravel 10 migration, then we will create routes, controller, view, and model files for the product module. we will use bootstrap 5 for designing.
 

## Quickstart

1. Make sure you have composer installed.
```bash
composer create-project laravel/laravel example-app
```

2. Database Configuration in .env file.
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=here your database name(blog)
DB_USERNAME=here database username(root)
DB_PASSWORD=here database password(root)
```

3. Create Migration
```bash
php artisan make:migration create_products_table --create=products
```

```bash
php artisan migrate
```

4. Create Controller and Model
```bash
php artisan make:controller ProductController --resource --model=Product
```

5. Add Resource Route in routes/web.php
```bash
Route::resource('products', ProductController::class);
```

6. Add Blade Files
```bash
1) layout.blade.php

2) index.blade.php

3) create.blade.php

4) edit.blade.php

5) show.blade.php
```

6. Run Laravel App
```bash
php artisan serve
``` 

7. Now, Go to your web browser, type the given URL and view the app output:
```bash
http://localhost:8000/products
``` 


