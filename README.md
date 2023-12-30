## Laravel-localize - a small Laravel package that allows to use composite primary keys.

### Installation:

 - composer require keasy9/laravel-composite-pk

### Usage:

    class Post extends Model
    {
        use HasCompositePrimaryKey;

        protected $primaryKey = ['author_id', 'category_id'];
        public $incrementing = false;

        //...
    }
