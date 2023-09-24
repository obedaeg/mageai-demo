# mageai-demo
This is a demo to use Mage Ai

## Get Started

This demo consist in Mage Ai docker container, and postgresql, this will help us to test the habilities that mage ai provide.

### First Step
As stated in the documentation, change the file `dev.env` for only `.env` and build the containers with

```bash
docker-compose build
```

### Second Step

Lets kick start the whole project by starting the compose configuration

```bash
docker-compose up
```

You will see that you can access mage.ai in the port `6789` and you can also access postgresql db with the `user: test` and `pass: test123` over the database `test`.

### Final Step

Create your ETL process, a quick example you can use the following CSV file:

- https://data.lacity.org/api/views/2nrs-mtv8/rows.csv?accessType=DOWNLOAD

and here is the mapping of the columns

```python
COLUMNS ={
    "DR_NO": "dr_no",
    "Date Rptd": "date_rptd",
    "DATE OCC": "date_occ",
    "TIME OCC": "time_occ",
    "AREA": "area",
    "AREA NAME": "area_name",
    "Rpt Dist No": "rpt_dist_no",
    "Part 1-2": "part_1_2",
    "Crm Cd": "crm_cd",
    "Crm Cd Desc": "crm_cd_desc",
    "Mocodes": "mocodes",
    "Vict Age": "vict_age",
    "Vict Sex": "vict_sex",
    "Vict Descent": "vict_descent",
    "Premis Cd": "premis_cd",
    "Premis Desc": "premis_desc",
    "Weapon Used Cd": "weapon_used_cd",
    "Weapon Desc": "weapon_desc",
    "Status": "status",
    "Status Desc": "status_desc",
    "Crm Cd 1": "crm_cd_1",
    "Crm Cd 2": "crm_cd_2",
    "Crm Cd 3": "crm_cd_3",
    "Crm Cd 4": "crm_cd_4",
    "LOCATION": "location",
    "Cross Street": "cross_street",
    "LAT": "lat",
    "LON": "lon"
    }
```

Have fun!
