---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fd7284fbc6204353432a30c97e4657e6b9206b7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subjectRightsRequest = {
  '@odata.type': '#microsoft.graph.subjectRightsRequest',
  internalDueDateTime: '2021-08-30T00:00:00Z'
};

await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}')
    .update(subjectRightsRequest);

```