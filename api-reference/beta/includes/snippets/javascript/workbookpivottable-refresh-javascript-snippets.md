---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2214e19980bba6150c95cfdbd784ea79f437031
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781519"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh')
    .version('beta')
    .post();

```