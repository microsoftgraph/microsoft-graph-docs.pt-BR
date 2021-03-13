---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5b3803124e612be3063f9ed36aa94433bbd9fd5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .delete();

```