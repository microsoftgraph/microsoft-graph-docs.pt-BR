---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462b6fe2c91155e0a849710e8da766385b52ca26
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/recent')
    .version('beta')
    .get();

```