---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36b7c783796351e28d9f00dfcfe124fd49f6c56f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear')
    .version('beta')
    .post();

```