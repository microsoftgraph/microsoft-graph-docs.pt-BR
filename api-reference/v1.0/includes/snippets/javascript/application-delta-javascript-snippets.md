---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9ac169581a7943ea2b806426d311aeaaf306d88
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/applications/delta')
    .get();

```