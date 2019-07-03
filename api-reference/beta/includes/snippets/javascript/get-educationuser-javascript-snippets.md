---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a1252b80b1db04e1631397cd73d3fa0ed97db09
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/13012')
    .version('beta')
    .get();

```