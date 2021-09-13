---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffdfd3a4338c5e2e8d4bd807fb7223da217cf46eeace62733ae38ad37bc65729
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acquireAccessToken = {
  credentials: [
    {
      '@odata.type': 'microsoft.graph.synchronizationSecretKeyStringValuePair'
    }
  ]
};

await client.api('/applications/{applicationsId}/synchronization/acquireAccessToken')
    .version('beta')
    .post(acquireAccessToken);

```