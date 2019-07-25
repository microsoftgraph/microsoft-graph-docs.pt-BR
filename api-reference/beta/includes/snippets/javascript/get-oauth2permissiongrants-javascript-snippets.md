---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecc360f08bc57f2417da3b3191f2f8312d89a74b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/oAuth2Permissiongrants')
    .version('beta')
    .get();

```