## MCPro is abbreviation of Municipalities, Cities and Provinces in the Philippines

Installation:

- composer install
- php artisan vendor:publish
- set your database credentials `.env`
- php artisan key:generate
- composer dump-autoload && php artisan migrate --seed && php artisan serve
- go to http://localhost:8000/api/v1/country

### Endpoints

- `/api/v1/country` - List all the countries

- `/api/v1/country/{country_id}` - Details of the country ( PH is id:169 )

- `/api/v1/country/{country_id}/province` - List all the provinces of the country (Currently for the PH)

- `/api/v1/country/{country_id}/province/{province_id}` - Details of the province

- `/api/v1/country/{country_id}/province/{province_id}/city` - Cities ( and Municipalities) of the province

- `/api/v1/country/{country_id}/province/{province_id}/city/{city_id}` - Details of the city

- `/api/v1/country/{country_id}/province/{province_id}/city/{city_id}/barangay` - List all the barangays of the City (or Municipality)
