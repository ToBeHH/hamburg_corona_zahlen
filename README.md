# run analysis
Run it in binder: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ToBeHH/hamburg_corona_zahlen/HEAD)

# get all the data
```
sudo gem install wayback_machine_downloader
wayback_machine_downloader https://www.hamburg.de/corona-zahlen -s -c 5
```

# Update data
1. Install [pipenv](https://pipenv.pypa.io/en/latest/) via `pip install --user pipenv`
2. Install missing files via `pipenv install`
3. Activate the virtual env via `pipenv shell`
4. Update the data via `python3 extract_data_from_archive.py`