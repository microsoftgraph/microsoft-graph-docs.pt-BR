---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e35e21714d8f6469ff91016b7f536e514b924064
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}')
    .delete();

```