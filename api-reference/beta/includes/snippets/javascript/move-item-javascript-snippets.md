---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e181e8fd1ceb819dbfe20831d286f7ba4c87853
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: 'new-parent-folder-id'
  },
  name: 'new-item-name.txt'
};

await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update(driveItem);

```