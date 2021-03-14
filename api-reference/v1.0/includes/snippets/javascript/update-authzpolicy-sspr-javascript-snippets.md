---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7db0b686b2ba3d466f20d1e3605ccf6a43c78704
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   allowedToUseSSPR: true
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```