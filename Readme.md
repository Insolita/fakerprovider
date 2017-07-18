Faker Shop-data provider (Russian only)
-----------------------

Генератор категорий, назвний товаров, материалов, размеров, бренвдов и аттибутов товаров

```php
 $faker = \Faker\Factory::create();
 $faker->addProvider(insolita\faker\ShopProvider::class);

 $faker->productUnit();
 $faker->productModel();
 $faker->productSize2d();
 $faker->productSize3d();
 $faker->productTitle();
 $faker->productCategory();
 $faker->productMaterial();
 $faker->productAttribute();
 $faker->productTrademark();

```