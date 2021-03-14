---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d01d41bffd4e5f55141f744d32091592f2aa8b1f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/servicePrincipals/{id}/createdObjects')
    .get();

```