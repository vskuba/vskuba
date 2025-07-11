## Technical task

### Brief description

Develop a web service for managing cinema tickets.

Stack technologies which must be involved on project:
- Docker, PHP (>= 7.4), Mysql, Redis, Nginx 
- Framework: Symfony (^4|5|6)
- Architecture pattens:  DDD, MVC
- Code style: PSR
- Code patterns (at least factory symfony in-built)
- DB entities: films, tickets, visitors (Mysql, Doctrine)
- DB migrations includes indexes for main queries
- Tests: few tests (Behat + Phpunit)
- Cache: Redis (simple cache)
- API UI: swagger

### Need to implement:

1. microservice by rest API with Swagger UI main API-ends:
- movies: CRUD
- movie's session CRUD (price) 
- visitor CRUD, name
- visitor buy/cancel ticket
- statistics total by day, week: tickets, resume session sum
- statistics total by visitor: tickets (buy/cancel), sums

2. Single page which display:
- list of movies with sessions
- the session has info about visitors which bought tickets ant total sum
- simple form for register new visitor
- simple form for the visitor buy/cancel ticket