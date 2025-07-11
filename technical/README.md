## Technical task

### Brief description

Develop a web service for managing cinema tickets.

Stack technologies which must be involved on project:
- Docker, PHP (>= 7.4), Mysql, Redis, Nginx 
- Framework: Symfony (^4|5|6)
- Architecture pattens:  DDD, MVC
- Code style: PSR
- Code patterns: Factory (symfony in-built), Decorator (symfony in-built), Strategy 
- DB entities: films, tickets, visitors (Mysql, Doctrine)
- DB migrations includes indexes for main queries
- Tests: few tests (Behat + Phpunit)
- Cache: Redis (simple cache)
- API UI: swagger


### Need to implement:

1. microservice by rest API with Swagger UI main API-ends:
- movies: CRUD
- movie's session CRUD
- ticket to session: buy/cancel, price 
- visitor: CRUD, (probability of visiting each movie session 92-98%)
- statistics by day, week: tickets, visitors visited/missed movies, spent money

2. Single page which display:
- list of movies with sessions
- the session has info about visitor which bought tickets ant total sum
- simple form for buy ticket