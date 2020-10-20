---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b12472c937c0dae48bc89d9b768456d0129e3cb2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/memberOf')
    .version('beta')
    .get();

```