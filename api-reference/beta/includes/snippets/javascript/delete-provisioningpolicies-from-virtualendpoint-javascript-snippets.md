---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f68168872df72e55d4fc4b20d1ee5f79603f9b41
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .delete();

```