---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10fa2024ebfcf924ab321f8340092e80f59fc6d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/emails/{id}')
    .version('beta')
    .delete();

```