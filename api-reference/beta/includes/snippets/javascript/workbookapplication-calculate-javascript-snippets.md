---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24e3db47dbc7b9480e86c282070f25dc6c70660c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calculate = {
  calculationType: "calculationType-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/application/calculate')
    .version('beta')
    .post(calculate);

```