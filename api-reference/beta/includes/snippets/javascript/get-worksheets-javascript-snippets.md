---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 410ee3e8a737a8290a519f05c2d4a78d722c47d3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498652"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets')
    .version('beta')
    .get();

```