---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4716ec59e2d0145d388c65186f365fe35e9868a4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .get();

```