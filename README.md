# pyramid_wiki
   - A wiki using Pyramid + SQLAlchemy: https://pyramid.readthedocs.io/en/stable/tutorials/wiki2/index.html

### How to Run It  
        
  - Execute the program using:

```bash
pserve development.ini
```
### Virtual environment
  - Testing against Python 3.7 to support data classes.  
```bash 
virtualenv -p python3.7 venv
```

### How to Run the Unit Tests
1. Activate the virtualenv
    ```bash
       source venv/bin/activate
    ```
1. Install the project in editable mode with its testing requirements:
    ```bash
       cd PROJECT_ROOT/pyramid_wiki/tutorial
       pip install -e ".[testing]"       
    ```
1. Initialize and upgrade the database using Alembic.

    - Generate your first revision.

        ```bash 
           alembic -c development.ini revision --autogenerate -m "init"
        ```

    - Upgrade to that revision.
       ```bash
          alembic -c development.ini upgrade head
       ```

1. Load default data into the database using a script.
    ```bash
       initialize_tutorial_db development.ini
    ```

1. Run the tests:
    ```bash
       cd PROJECT_ROOT/pyramid_wiki/tutorial
       pytest
    ```
1. Run your project.
   ```
       pserve development.ini
   ```
### Key Dependencies

### Future Enhancements
