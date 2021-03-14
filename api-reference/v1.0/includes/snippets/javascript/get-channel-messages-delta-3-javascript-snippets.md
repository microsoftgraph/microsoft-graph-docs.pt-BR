---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32d93f8788fb3101513a1d39b8af0db711f40399
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyODcyMzY2NzgmcGFnZVNpemU9MjA=')
    .get();

```