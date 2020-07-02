# GRPC example using Python

## Running this project

### Clone this project

```bash
git clone https://github.com/shahedex/grpc-py.git
```

### Create and activate virtualenv

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install the requirements

```bash
pip install -r requirements.txt
```

### Run the GRPC server

```bash
python greeter_server.py
```

### Run the GRPC client to get responses

```bash
python greeter_client.py
```

## Updating to new proto file

```bash
python -m grpc_tools.protoc -I . --python_out=. --grpc_python_out=. greeter_service.proto
```
