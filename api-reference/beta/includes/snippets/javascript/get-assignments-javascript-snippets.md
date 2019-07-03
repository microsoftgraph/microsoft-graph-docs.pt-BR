---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df16d55be836c7cea323f143396ca84f258788d4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/assignments')
    .version('beta')
    .get();

```