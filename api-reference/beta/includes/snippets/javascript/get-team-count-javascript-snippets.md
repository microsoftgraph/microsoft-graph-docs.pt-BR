---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 313021ca0a25e326cc4e946323c2849804c50015
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .search('displayName:Team')
    .get();

```