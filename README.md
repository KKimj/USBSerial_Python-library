# USBSerial_Python-library
USBSerial_Python-library


https://pypi.org/project/USBSerial

## Getting Started

### Installation
```
$ pip install USBSerial
```

## Usage

### Import
```python
from usbserial import USBSerial
```

### Examples
```python
from usbserial import USBSerial
device = USBSerial(port = 'ttyUSB0', baudrate = 115200, timeout = 3, open = True)
print(device.readline())
print(device.read(size = 1))
```


## Dev

### Build
```
$ python3 -m build
```

### Local test
```
$ pip install -e .
```

#### Build and Local test
```
$ python3 -m build && pip install -e . && python
```

### Release
```
$ python -m twine upload dist/*
```

