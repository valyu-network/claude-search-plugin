# Answer with Fast Mode

Enable fast mode for quicker responses with lower latency.

```typescript
import { Valyu } from "valyu-js";

const valyu = new Valyu(YOUR_VALYU_API_KEY_HERE);

const data = await valyu.answer({
  query: "current market trends in tech stocks",
  fastMode: true,
  dataMaxPrice: 30.0
});

console.log(data.contents);
```

```python
from valyu import Valyu

valyu = Valyu()

data = valyu.answer(
    query="current market trends in tech stocks",
    fast_mode=True,
    data_max_price=30.0
)

print(data["contents"])
```

## CLI
```bash
scripts/valyu answer "current market trends in tech stocks" --fast
```

## When to Use Fast Mode

- Quick lookups and simple questions
- Time-sensitive queries
- When lower cost is preferred
- Real-time applications
