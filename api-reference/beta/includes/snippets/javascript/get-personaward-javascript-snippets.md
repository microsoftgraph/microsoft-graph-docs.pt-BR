---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc89bb4176644b4da1663280c202f4f1cf2d82f3
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/awards/{id}')
    .version('beta')
    .get();

```