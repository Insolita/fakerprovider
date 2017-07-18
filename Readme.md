Faker Shop-data provider (Russian only)
-----------------------

Генератор категорий, назвний товаров, материалов и аттибутов товаров

```php
 $faker = \Faker\Factory::create();
 $faker->addProvider(insolita\faker\ShopProvider::class);

 $faker->productTitle();
 $faker->productCategory();
 $faker->productMaterial();
 $faker->productAttribute();
```