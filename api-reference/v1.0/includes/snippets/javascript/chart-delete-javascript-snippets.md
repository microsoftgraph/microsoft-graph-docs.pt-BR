---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1537a64fc01d6cff7fc13081c3f44bb53e45d6d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .delete();

```