---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 963662a959ef37341b6333e8c992d7f2ff8a79ad
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberGroups')
    .version('beta')
    .post(String);

```