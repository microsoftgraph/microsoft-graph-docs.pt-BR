---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 881332f03fd3bc82688bc152f14cbb9cb12874c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793737"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _delete = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/delete')
    .post(_delete);

```