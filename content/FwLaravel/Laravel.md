```php
class IssueProjection extends Projection  
{  
    use HasFactory;  
  
//    public int $penalty;  
  
    protected $guarded = [];
```
- $issue를 find method를 통해 받아오고 penalty를 접속하려고 하면 initialized 되기 전에 접속하면 안된다고 에러가 발생한다

# Database
### migrate 관련 명령어
- step 옵션을 주지 않으면 모든 마이그레이션 파일에 대해 실행된다
`php artisan migrate`
`php artisan migrate:rollback --step=1`

- 새로 다시 마이그레이션하기
`php artisan migrate:refresh`
`php artisan migrate:reset`

- db 채우기
`php artisan db:seed`

### migration file 작성
- dropForeign을 사용하면 외래키 설정만 제거할 수 있다
예시: `$table->dropForeign(['user_id']);`
