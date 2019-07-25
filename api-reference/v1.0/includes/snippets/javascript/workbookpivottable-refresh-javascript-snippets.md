---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 065f298947d150d1b37698aa200a1fa0447e4c24
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh')
    .post();

```