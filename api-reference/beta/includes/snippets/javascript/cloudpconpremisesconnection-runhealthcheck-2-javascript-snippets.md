---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca2dd2536ceb8b6b8f6ea09aee26f7894aff85cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947592"
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