---
layout: post
title: Фиксы тестов для использования stub в sinon
---

Особенность экспортирования модулей для вызова их фукнций

```
// экспортируем модули, так как если будем экспортировать функции напрямую из модулей, их нельзя застабить в sinon
// и в тестах все равно будут вызываться функции напрямую
const documentTerminate = require('../../../../domain/documents-terminate')
const documentJoin = require('../../../../domain/documents-join')
```
