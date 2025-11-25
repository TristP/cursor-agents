# Shared Resources

This directory contains shared code, utilities, and resources that can be used across all agent projects.

## Contents

- `utils/` - Shared utility functions
- `config/` - Shared configuration files
- `data/` - Shared data files
- `docs/` - Shared documentation

## Usage

Import shared resources in your agent projects as needed.

### Example (Python):
```python
import sys
sys.path.append('../shared')
from utils import helper_function
```

### Example (Node.js):
```javascript
const helper = require('../shared/utils/helper');
```

