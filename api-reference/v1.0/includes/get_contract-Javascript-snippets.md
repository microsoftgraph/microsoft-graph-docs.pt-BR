---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4716ec59e2d0145d388c65186f365fe35e9868a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contracts')
    .get();

```