# Housing Market
This is a dummy project

# Usage:
With Docker:
1. `docker-compose up`
2. copy this URL into your web browser: http://admin:default@127.0.0.1:9999/listings

Without Docker:

1. `virtualenv env`
2. `source env/bin/activate`
3. `pip install pip setuptools --upgrade`
4. `pip install -r requirements.txt`
5. `python setup.py develop`
6. `pyhton app/common/init_db.py`
7. `python app/api.py`

# Contribution
If you want to see your modifications, use `docker-compose up --force-recreate --build`.

# ToDo
1. Make sure `/listings:search` returns proper results.
2. Add `tram_stop` and `bus_stop` to the amenities (datasets are available on the [open data website](https://data.bordeaux-metropole.fr/themes))
3. Make sure `Listing` table is refreshed every 15 minutes.
4. Store user's most recent search and send a notification to their email if a new listing that matches his critirias appears.
