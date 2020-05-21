---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 094dadf55b317d33b13401f7c0a78355d467cb9b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/owners')
    .get();

```