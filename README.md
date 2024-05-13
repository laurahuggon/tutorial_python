# Python tutorials

## Virtual environment (venv) set-up
Every time you made a new project, you should make a new virtual environment.
1. In PyCharm, press `Cmd` + `,` to bring up settings.
2. Click `Project: ...` > `Python Interpreter` > `Add Interpreter` > `Add Local Interpreter`.
3. Select `Virtualenv Environment` > `New`.
4. Make sure that `Base Interpreter` path is: "/Users/.../mambaforge/bin/python3.10".
5. Click `OK` > `Apply` > `OK`.
6. Or, enter into terminal:
```
python3 -m venv venv    # This makes the environment
source venv/bin/activate    # This activates the environment
```
7. If you want to deactivate the environment:
```
deactivate  # This deactivates the environment
```

## Installing packages
1. Make `requirements.txt`.
2. Add any packages required for this project.
3. Go to Terminal.
4. Check that you are in (venv).
5. In terminal, run:
```
pip install -r requirements.txt
```
6. Alternatively, `pip install [package_name]` then add package name to `requirements.txt`.
7. To uninstall, use `pip uninstall [package_name]` and remove from `requirements.txt`.

## Export to HTML
To export a Jupyter notebook to HTML, run the following code within the notebook:
```
!jupyter nbconvert --to html [notebook_name].ipynb
```