---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c79462e26bfd1cde50c481c4f85bbc06a27092b5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2cUserFlows/{id}/identityProviders')
    .version('beta')
    .get();

```