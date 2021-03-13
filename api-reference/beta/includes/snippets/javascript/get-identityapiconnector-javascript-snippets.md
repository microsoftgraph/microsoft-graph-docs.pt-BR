---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99493eeb64aa33713cb20b270bc1c95e73d500dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityApiConnector = await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .get();

```