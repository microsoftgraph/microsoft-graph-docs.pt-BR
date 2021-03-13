---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 095878df1758182099e0383c0025953fd06d2346
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/names')
    .version('beta')
    .get();

```