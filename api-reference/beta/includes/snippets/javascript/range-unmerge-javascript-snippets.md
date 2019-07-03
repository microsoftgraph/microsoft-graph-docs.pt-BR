---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20a4cf0e11009ae5d23aa6851e639dff973ea742
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518310"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/unmerge')
    .version('beta')
    .post();

```