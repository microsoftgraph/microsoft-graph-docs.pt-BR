---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3eca665a187cabab14fbd0f1afea081a9fcc00d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/{id}/channels/{id}/messages/delta')
    .version('beta')
    .top(2)
    .get();

```