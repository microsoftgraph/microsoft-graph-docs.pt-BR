---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f8c2c166002f927e6866828d84f53e046d2409b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789131"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let skillProficiency = await client.api('/me/profile/skills/{id}')
    .version('beta')
    .get();

```