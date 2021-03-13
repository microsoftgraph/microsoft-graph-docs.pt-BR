---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 806a9ca831d88fa7bb45e9ee4c64748c56ae75af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/awards/{personAwardId}')
    .version('beta')
    .delete();

```