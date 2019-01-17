| Method    | URI                                     | Name             | Action                                         | Middleware   |
| --------- | --------------------------------------- | ---------------- | ---------------------------------------------- | -------------|
| GET|HEAD  | /                                       |                  | Closure                                        | web          |
| GET|HEAD  | api/products                            | products.index   | App\Http\Controllers\ProductController@index   | api          |
| POST      | api/products                            | products.store   | App\Http\Controllers\ProductController@store   | api          |
| GET|HEAD  | api/products/{product}                  | products.show    | App\Http\Controllers\ProductController@show    | api          |
| PUT|PATCH | api/products/{product}                  | products.update  | App\Http\Controllers\ProductController@update  | api          |
| DELETE    | api/products/{product}                  | products.destroy | App\Http\Controllers\ProductController@destroy | api          |
| GET|HEAD  | api/products/{product}/reviews          | reviews.index    | App\Http\Controllers\ReviewController@index    | api          |
| POST      | api/products/{product}/reviews          | reviews.store    | App\Http\Controllers\ReviewController@store    | api          |
| GET|HEAD  | api/products/{product}/reviews/{review} | reviews.show     | App\Http\Controllers\ReviewController@show     | api          |
| PUT|PATCH | api/products/{product}/reviews/{review} | reviews.update   | App\Http\Controllers\ReviewController@update   | api          |
| DELETE    | api/products/{product}/reviews/{review} | reviews.destroy  | App\Http\Controllers\ReviewController@destroy  | api          |
| GET|HEAD  | api/user                                |                  | Closure                                        | api,auth:api |