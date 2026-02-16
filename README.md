# Pipenv Test Case 8: setup.cfg Fallback

## What This Tests
Tests detection of Python version from setup.cfg when no higher-priority files specify a version.

## Expected
>=3.9 found through SetupCfgPythonRequires

## Files
- `Pipfile` - No requires section
- `setup.cfg` - Contains `python_requires = >=3.9`

## Expected Behavior
Your version detection tool should detect **Python >=3.9** from setup.cfg.

## Priority
This is the **sixth priority** detection method for Pipenv projects.

## Note
setup.cfg serves as a fallback for Python version detection in projects that use it for packaging configuration.
