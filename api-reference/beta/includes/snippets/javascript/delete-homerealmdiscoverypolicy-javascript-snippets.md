---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee7d2d6dfda11c611bde1d2ef9936cda5971f52f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .delete();

```