---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1dcb9976c7e4abcc132bb7d3f92f40a45c186abe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/revokeSignInSessions')
    .version('beta')
    .post();

```