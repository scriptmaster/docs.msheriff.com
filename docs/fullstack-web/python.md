#

### FastAPI

Then open OpenAPI docs with: /docs
```
from fastapi import FastAPI

app = FastAPI()


@app.get("/")
def read_root():
    return {"Hi": "There"}

```

#### subprocess

For a webhook
```
    whoami = subprocess.run(['whoami'], capture_output=True)
    pull_output  = subprocess.run('git -C /repo/dir/ pull --autostash --rebase=true'.split(), capture_output=True)
    # ...
    return {'whoami': whoami, 'pull': pull_output}
```
