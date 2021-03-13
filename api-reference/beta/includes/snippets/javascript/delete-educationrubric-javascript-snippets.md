---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b9c652da6f7ee72197e188338a8c3120c39fa4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .delete();

```