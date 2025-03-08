---
layout: post
title: Concurrency in application
---

Business process that need to be a transaction, which success or fail but not in middle state.

With short transaction, which is **system transaction**, database provide mechanism for this. However, with business logic that last hour, holding database transaction would decrease performance, which is the first reason we use concurrent processing (enhance performance)

⇒ With **business transaction** like this, we must try to break it into multiple **system transaction**

They are still the same problem:

- Lost update (handle by locking or change business logic to not override data but update it by adding or minus)
- Dirty read
- Inconsistent read
- Phantom read
The 3 later problems due to lack of isolation between transactions.

System transaction have isolation level

While with business transaction, we use optimistic concurrency process, pessimistic concurrency process. If not success, we may need to skip concurrency and use event driven approach.
