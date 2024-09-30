---
title: PHP
tags:
---
# string
- string 안에 변수 값을 집어넣는 방법

## anonymous classses
```php
public function test_somthing(): void
{
    $dto = new class(
        ['arrayOfInts' => [1, 2]]
    ) extends DataTransferObject {
        /** @var int[] */
        public array $arrayOfInts;
	};
}
```
## WeakMap
- 참조가 사라지면 가비티 콜렉팅이 되도록 하는 map
```php
class EntityCache
{
    public function __construct(
	    private WeakMap $cache
	) {}

	public function getSomethingWithCaching(object $object): object
	{
		if (! isset($this->cache[$object])){
			$this->cache[$object] = $this
				->computeSomethingExpensive($object);
		}
		
		return $this->cache[$object];
	
	}
}
```
# array
## how do you append to an array?
```php
$array = array("apple", "banana", "cherry");
$array[] = "date"; // Appending "date" to the array

print_r($array);
```
