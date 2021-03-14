---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 348c7cfb8c7613d043602ce823aca9fc25ec4011
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange')
    .get();

```