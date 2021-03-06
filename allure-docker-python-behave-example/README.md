# PYTHON BEHAVE DEMO PROJECT USING ALLURE

## INSTALLATION
- Download Python 3
https://www.python.org/downloads/

- Check Python version
```sh
python3 --version
```
- Go to project
- Install dependencies

```sh
pip3 install -r requirements.txt
 ```

## USAGE
Execute Allure Docker Service from this directory
```sh
docker-compose up -d allure
```
- Verify is Allure report is working. 
- Go to -> http://localhost:5050/latest-report

Each time you run tests, the Allure report will be updated.
Execute tests:
```sh
behave -f allure_behave.formatter:AllureFormatter -o ./allure-results
```

See documentation here: https://github.com/fescobar/allure-docker-service


## DEVELOPER USAGE
Freeze dependencies when you update some of them
```sh
pip freeze > requirements.txt
```
https://blog.miguelgrinberg.com/post/the-package-dependency-blues
