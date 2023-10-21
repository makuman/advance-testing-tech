# advance-testing-tech
This is repo for advance testing

## setup project
1. Create and source virtualenv
virtualenv ~/.advanced-testing
source ~/.advanced-testing/bin/activate

2. Create Source folder
```bash
touch makefile && touch requirements.txt && touch hello.py && touch test_hello.py
```

3. Populate `MakeFile`

```bash
install:
	pip install --upgrade pip &&\
		pip install -r requirements.txt

test:
	python -m pytest -vv --cov=hello --cov=hellocli test_hello.py

lint:
	pylint --disable=R,C hello.py hellocli.py

all: install lint test
```

### How to debug 

* Print
* pdb
* testing


