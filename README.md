# example_package_chenglim
test package as template for creating pypi packages

## Generating Distribution Archives
Run the following to generate a dist directory
python -m build

## Uploading package to test repository
python -m twine upload --repository testpypi dist/*

## Uploading package to pypi
python -m twine upload dist/*

## Installing package from test repository
python -m pip install --index-url https://test.pypi.org/simple/ --no-deps example_package_chenglim

## Installing package from pypi
python -m pip install --no-deps example_package_chenglim