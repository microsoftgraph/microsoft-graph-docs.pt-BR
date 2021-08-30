---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 911e71263b5b466e731fb6865aa3654a6ba4dd7e9a77f4880fe451bb15547c21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupIds-value'
  ]
};

await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .version('beta')
    .post(string);

```