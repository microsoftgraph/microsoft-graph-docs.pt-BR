---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84b82dcb6546990bfc8753f81d28d7335cdeadce
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603296"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles')
    .version('beta')
    .get();

```