---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f029a8bd7f46c712cc7623d76f4c59dff97eba7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/estimateStatistics')
    .version('beta')
    .post();

```