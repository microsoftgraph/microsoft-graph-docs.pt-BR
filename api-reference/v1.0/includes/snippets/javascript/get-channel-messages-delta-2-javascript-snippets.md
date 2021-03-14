---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8532479d179a742a437c9dfbcd71b943053b1503
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chatMessage = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .skiptoken('c3RhcnRUaW1lPTE1NTEyMTUzMjU0NTkmcGFnZVNpemU9MjA=')
    .get();

```