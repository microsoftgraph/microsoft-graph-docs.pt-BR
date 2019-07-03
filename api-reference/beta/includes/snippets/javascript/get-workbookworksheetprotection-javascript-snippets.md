---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 305c0ca0d0ea74cca054c228fa730c52f95dac87
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection')
    .version('beta')
    .get();

```