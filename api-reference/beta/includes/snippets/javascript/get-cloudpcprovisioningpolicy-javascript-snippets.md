---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 273dfa8b3b499dacd50387a42509cc695deb7c27
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .expand('assignments')
    .get();

```