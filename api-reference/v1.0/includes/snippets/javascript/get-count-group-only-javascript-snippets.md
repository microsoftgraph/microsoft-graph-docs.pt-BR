---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 858baec23eb7053f903ddee43010db45497b9e3b
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903752"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count')
    .header('ConsistencyLevel','eventual')
    .get();

```