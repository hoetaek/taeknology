---
tags:
  - entry
---
[[laravel database]]
[[laravel-event-sourcing]]


```php
class IssueProjection extends Projection  
{  
    use HasFactory;  
  
//    public int $penalty;  
  
    protected $guarded = [];
```
- $issue를 find method를 통해 받아오고 penalty를 접속하려고 하면 initialized 되기 전에 접속하면 안된다고 에러가 발생한다
