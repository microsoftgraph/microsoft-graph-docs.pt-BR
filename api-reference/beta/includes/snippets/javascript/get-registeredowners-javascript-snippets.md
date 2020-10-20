---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e08ebe113c02f5b7b2fda948eb4d8c66e53361d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners')
    .version('beta')
    .get();

```