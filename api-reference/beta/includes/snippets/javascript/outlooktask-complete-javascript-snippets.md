---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21be991423bc375e0f4075cdebd7394b2468c23f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete')
    .version('beta')
    .post();

```