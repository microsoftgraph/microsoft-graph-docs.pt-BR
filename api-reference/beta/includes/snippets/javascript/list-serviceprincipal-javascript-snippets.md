---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b5b3fc817ebe14ece2b61fab447d0069536f364
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/serviceprincipals')
    .version('beta')
    .get();

```