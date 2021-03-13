---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 590c97011dfbbc79b33c3eb89d499e91ac1455d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771236"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .delete();

```