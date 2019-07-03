---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0be28814ca4509e5d5576e040ba41d5ae8140750
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518877"
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