---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca2dd2536ceb8b6b8f6ea09aee26f7894aff85cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks')
    .version('beta')
    .post();

```