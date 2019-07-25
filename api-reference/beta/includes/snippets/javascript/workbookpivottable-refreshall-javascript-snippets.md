---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0be28814ca4509e5d5576e040ba41d5ae8140750
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll')
    .version('beta')
    .post();

```