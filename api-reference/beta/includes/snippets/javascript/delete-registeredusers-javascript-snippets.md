---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa6ca413b474c098b73cc2417cb774a8150ed0fe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredUsers/{id}/$ref')
    .version('beta')
    .delete();

```