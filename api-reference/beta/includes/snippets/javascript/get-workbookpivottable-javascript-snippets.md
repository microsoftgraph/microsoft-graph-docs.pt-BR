---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddf774784a31ff8a1b7305288010d09345b41ec5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookPivotTable = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .version('beta')
    .get();

```