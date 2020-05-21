---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ccfd456da96ff60ee58f041dea76626727b20486
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333443"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: "65415bb1-9267-4313-bbf5-ae259732ee12",
};

let res = await client.api('/serviceprincipals')
    .version('beta')
    .post(servicePrincipal);

```