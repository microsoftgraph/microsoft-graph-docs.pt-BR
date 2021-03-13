---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62637a7aa7a0e72ad39ab426609787a792aac19c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods/{id}')
    .version('beta')
    .delete();

```