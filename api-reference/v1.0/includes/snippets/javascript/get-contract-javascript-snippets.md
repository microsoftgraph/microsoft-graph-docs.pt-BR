---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4716ec59e2d0145d388c65186f365fe35e9868a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .get();

```