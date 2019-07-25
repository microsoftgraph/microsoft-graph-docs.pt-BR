---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdcb54069667118af908b12f588d7344d38c2967
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles/{id}')
    .version('beta')
    .get();

```