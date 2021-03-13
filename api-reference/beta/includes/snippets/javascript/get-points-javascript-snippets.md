---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12c6ff0622894e19b77a1fa70eba992032ab9310
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let points = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points')
    .version('beta')
    .get();

```