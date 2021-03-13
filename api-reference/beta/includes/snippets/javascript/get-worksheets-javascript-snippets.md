---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9581bd497e1ddfbfd850907176c94155c6abffa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806620"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let worksheets = await client.api('/me/drive/items/{id}/workbook/worksheets')
    .version('beta')
    .get();

```