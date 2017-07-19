Faker Shop-data provider (Russian only)
-----------------------

Генератор категорий, назвний товаров, материалов, размеров, брендов и аттибутов товаров

```
  composer require "insolita\fakerprovider":"~1.0"
```

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

// in some cases, if you have faker instance as closure argument- add provider like
```php
$factory->define(\App\Modules\Shop\Product::class, function (Faker\Generator $faker) {
    $faker->addProvider(new \insolita\faker\ShopProvider($faker));
    //....
});

```