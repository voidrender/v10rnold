# v10rnold

Using node@10, install dependencies with yarn:
```
yarn
```

Next, install iOS dependencies:

```
cd ios && pod install
```

Then run the iOS app:

```
yarn ios
```

You should see this error:

```
fatal error: 'execution_context_id.hpp' file not found
#include "execution_context_id.hpp"
```
in `js_types.hpp`

**Update**: This error was addressed by switching to the npm repo instead of referencing github directly. (It was also updated to alpha.9 but I don't think that was the fix.)