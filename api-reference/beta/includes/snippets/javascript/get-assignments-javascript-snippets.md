---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df16d55be836c7cea323f143396ca84f258788d4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605704"
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