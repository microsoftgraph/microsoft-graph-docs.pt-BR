---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de97c734daded25931e5e0099f596be43e6e1eaa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/cloudPCs/{cloudPCId}/endGracePeriod')
    .version('beta')
    .post();

```