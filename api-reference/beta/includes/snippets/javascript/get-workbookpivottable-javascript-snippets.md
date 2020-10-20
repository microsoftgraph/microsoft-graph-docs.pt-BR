---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 750cda9395da59f9b7c216719883e2c262183445
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .version('beta')
    .get();

```