---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c961ca782110f8b71dc85d93991b00e49161840
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302274"
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
    .post(calculate);

```