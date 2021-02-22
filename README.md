# pyramid_wiki
   - A wiki using Pyramid + SQLAlchemy: https://pyramid.readthedocs.io/en/stable/tutorials/wiki2/index.html

### How to Run It  
        
  - Execute the program using:
  
  
      -  $ python main.py

### Virtual environment
  - Testing against Python 3.7 to support data classes.  
```bash 
virtualenv -p python3.7 gdprlib_venv
```

### How to Run the Unit Tests
1. Activate the virtualenv
    ```bash
       source venv/bin/activate
    ```
1. Install requirements as usual:
    ```bash
       cd PROJECT_ROOT/utils/pyramid_wiki
       pip install -r requirements/requirements.txt
       pip install -r requirements/test-requirements.txt
    ```
1. Run the tests:
    ```bash
       cd PROJECT_ROOT/utils/pyramid_wiki
       pytest
    ```
    
### Key Dependencies

### Future Enhancements
