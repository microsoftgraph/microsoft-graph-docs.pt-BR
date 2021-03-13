---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0eec45d54f0a5d1d9329277007089a5fd5971f5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/interests/{id}')
    .version('beta')
    .delete();

```