---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10e28a7d61d0270823663f7a06b6ec1d5e31daa8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/education/classes/11016/members')
    .version('beta')
    .get();

```