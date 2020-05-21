---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 488be4dae8fae79bff0f6b09956afd59048a951e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('hasMembersWithLicenseErrors+eq+true,')
    .select('id,displayName')
    .get();

```