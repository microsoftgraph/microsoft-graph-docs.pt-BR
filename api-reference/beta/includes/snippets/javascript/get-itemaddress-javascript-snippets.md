---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35c31f0e06e6cb66541f318ddb5ab1527d8777c2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/addresses/{id}')
    .version('beta')
    .get();

```