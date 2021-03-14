---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e63be77d920087451653e23945d2a8dde698879
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{user-id}')
    .delete();

```