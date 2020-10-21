---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c3392836fbef1a3ea2e4e07270db614d3ac1341
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables')
    .get();

```