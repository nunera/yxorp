***

# JsonType

Scalar Type Definition

The leaf values of any request and input values to arguments are
Scalars (or Enums) and are defined with a name and a series of coercion
functions used to ensure validity.

Example:

class OddType extends ScalarType
{
    public $name = 'Odd',
    public function serialize($value)
    {
        return $value % 2 === 1 ? $value : null;
    }
}

* Full name: `\App\GraphQL\Types\JsonType`
* Parent class: [`\GraphQL\Type\Definition\ScalarType`](../../../GraphQL/Type/Definition/ScalarType.md)



## Properties


### name



```php
public $name
```






***

### description



```php
public $description
```






***

## Methods


### __construct



```php
public __construct(string $name = null): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$name` | **string** |  |




***

### parseValue



```php
public parseValue(mixed $value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** |  |




***

### serialize



```php
public serialize(mixed $value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** |  |




***

### parseLiteral



```php
public parseLiteral(mixed $valueNode, array $variables = null): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$valueNode` | **mixed** |  |
| `$variables` | **array** |  |




***

### identity



```php
private identity(mixed $value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** |  |




***

### instance



```php
public static instance(): mixed
```



* This method is **static**.







***


## Inherited methods


### __construct



```php
public __construct(array $config = []): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** |  |




***

### id



```php
public static id(): \GraphQL\Type\Definition\ScalarType
```



* This method is **static**.







***

### string



```php
public static string(): \GraphQL\Type\Definition\ScalarType
```



* This method is **static**.







***

### boolean



```php
public static boolean(): \GraphQL\Type\Definition\ScalarType
```



* This method is **static**.







***

### int



```php
public static int(): \GraphQL\Type\Definition\ScalarType
```



* This method is **static**.







***

### float



```php
public static float(): \GraphQL\Type\Definition\ScalarType
```



* This method is **static**.







***

### listOf



```php
public static listOf(\GraphQL\Type\Definition\Type $wrappedType): \GraphQL\Type\Definition\ListOfType
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wrappedType` | **\GraphQL\Type\Definition\Type** |  |




***

### nonNull



```php
public static nonNull(callable|\GraphQL\Type\Definition\NullableType $wrappedType): \GraphQL\Type\Definition\NonNull
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wrappedType` | **callable&#124;\GraphQL\Type\Definition\NullableType** |  |




***

### isBuiltInType

Checks if the type is a builtin type

```php
public static isBuiltInType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### getAllBuiltInTypes

Returns all builtin in types including base scalar and
introspection types

```php
public static getAllBuiltInTypes(): \GraphQL\Type\Definition\Type[]
```



* This method is **static**.







***

### getStandardTypes

Returns all builtin scalar types

```php
public static getStandardTypes(): \GraphQL\Type\Definition\ScalarType[]
```



* This method is **static**.







***

### getInternalTypes



```php
public static getInternalTypes(): \GraphQL\Type\Definition\Type[]
```



* This method is **static**.


* **Warning:** this method is **deprecated**. This means that this method will likely be removed in a future version.






***

### overrideStandardTypes



```php
public static overrideStandardTypes(array&lt;string,\GraphQL\Type\Definition\ScalarType&gt; $types): mixed
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$types` | **array<string,\GraphQL\Type\Definition\ScalarType>** |  |




***

### isInputType



```php
public static isInputType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### getNamedType



```php
public static getNamedType(\GraphQL\Type\Definition\Type $type): ?\GraphQL\Type\Definition\Type
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### isOutputType



```php
public static isOutputType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### isLeafType



```php
public static isLeafType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### isCompositeType



```php
public static isCompositeType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### isAbstractType



```php
public static isAbstractType(\GraphQL\Type\Definition\Type $type): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### assertType



```php
public static assertType(mixed $type): \GraphQL\Type\Definition\Type
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **mixed** |  |




***

### getNullableType



```php
public static getNullableType(\GraphQL\Type\Definition\Type $type): \GraphQL\Type\Definition\Type
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$type` | **\GraphQL\Type\Definition\Type** |  |




***

### assertValid



```php
public assertValid(): mixed
```











***

### jsonSerialize



```php
public jsonSerialize(): string
```











***

### toString



```php
public toString(): string
```











***

### __toString



```php
public __toString(): string
```











***

### tryInferName



```php
protected tryInferName(): string|null
```











***


***

