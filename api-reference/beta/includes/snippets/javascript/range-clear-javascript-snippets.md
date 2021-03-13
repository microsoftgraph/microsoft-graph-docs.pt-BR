---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0df75a36a71e9627453da691a5b3ec1c92153085
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804875"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: 'applyTo-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .version('beta')
    .post(clear);

```