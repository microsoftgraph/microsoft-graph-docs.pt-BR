---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c85144aa5bd41c601446f80cd1ccb70b7c95cb2b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .version('beta')
    .get();

```