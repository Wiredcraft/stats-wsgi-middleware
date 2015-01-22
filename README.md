# Stats wsgi Middleware

The objectives are:

- build a uwsgi middleware that can be used on any python based uwsgi process (e.g. Flask, Django)
- track requests and responses stats into a redis database
- pip installable module (e.g. setup.py, requirements.txt)
- howto documentation / example to use and extract data

# Stats to track

- count of return code (2xx, 3xx, 4xx, 5xx), time-sensitive
    - 2xx: uri, source ip
    - 3xx: uri, source ip
    - 4xx: uri, source ip
    - 5xx: uri, source ip, raised exception message (no trace)

# Suggestions

- track stats in redis
- find proper redis value type to efficiently save / update stats

