---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81c0e73ecacba11858168cb345fc22d519726488
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies')
    .version('beta')
    .get();

```