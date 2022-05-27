---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58c08864e34266b875ff979f179cf4f76be49536
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719177"
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
    .version('beta')
    .update(subjectRightsRequest);

```