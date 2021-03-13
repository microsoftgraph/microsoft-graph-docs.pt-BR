---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2c421a93a67c9a9e64faf85bdd1cdc481e9fdd3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/notes/{id}')
    .version('beta')
    .delete();

```