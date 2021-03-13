---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e6b3d91374bb7498c011012568b660bfee1678a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permission = await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .get();

```