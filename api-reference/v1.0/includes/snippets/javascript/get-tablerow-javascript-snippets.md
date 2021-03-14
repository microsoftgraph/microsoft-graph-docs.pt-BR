---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9c6a349e53242ea5775f442ca869ec14790ea9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableRow = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .get();

```