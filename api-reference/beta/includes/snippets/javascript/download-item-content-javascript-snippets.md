---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad8561f37542b975ddce01946149e71d2af2ff99
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .get();

```