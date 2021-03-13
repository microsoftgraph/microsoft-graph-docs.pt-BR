---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c126f2168f2a56e3bdeeaabc8d875192b405e509
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookComment = await client.api('/drive/items/{id}/workbook/comments/{id}')
    .version('beta')
    .get();

```