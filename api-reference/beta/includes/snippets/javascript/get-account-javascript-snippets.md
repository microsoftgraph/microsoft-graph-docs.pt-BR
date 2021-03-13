---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3e70983214e2b1ca64dfe2244ee139eeecf279d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let account = await client.api('/me/profile/account')
    .version('beta')
    .get();

```