---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3420a4af45ba91845cfd0ce74996a275adda791
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .delete();

```