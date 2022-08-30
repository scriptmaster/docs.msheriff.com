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
