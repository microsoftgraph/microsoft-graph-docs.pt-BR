---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e8e0924629063e2f2686919ca31babe771dc2bcf451e49f099d20ec25d9407e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/plans/{plan-id}/buckets')
    .get();

```