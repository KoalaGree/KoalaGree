<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>
    
```python
​
from __future__ import annotations

import json
from dataclasses import asdict, dataclass


@dataclass
class ManCity:
    languages: tuple[str, ...] = ("Python", "PHP")
    databases: tuple[str, ...] = ("SQLAlchemy", "PostgreSQL")
    ongoing  : tuple[str, ...] = ("Ract", "Docker", "Node.js")

    def jsonify(self) -> str:
        return json.dumps(asdict(self), indent=4)


mancity = ManCity()
print(mancity.jsonify())
​
```
</h3>
