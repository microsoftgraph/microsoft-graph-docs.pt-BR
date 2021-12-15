---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 443e90fd9e884c1fd5d0cea1f2a0c6f2cc61afb1
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/tasks/lists/delta')
    .version('beta')
    .get();

```