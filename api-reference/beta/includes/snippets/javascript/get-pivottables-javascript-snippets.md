---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63a316d3ab449907da0cb272e0433277d0b03ed0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables')
    .version('beta')
    .get();

```