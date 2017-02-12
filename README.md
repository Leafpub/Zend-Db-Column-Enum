# Zend-Db-Column-Enum
ENUM Column Type for Zend Db

### Usage
```php
new Enum(
  'role', // field name
  ["'owner'","'admin'","'editor'","'author'"], // possible field values
  false, // isNullable
  'author' // deafult
)

$createTable = new \Zend\Db\Sql\Ddl\CreateTable('foo');
$createTable->addColumn(
  new Enum(
    'foo',
    ["'bar'", "'baz'"]
  )
);
```
