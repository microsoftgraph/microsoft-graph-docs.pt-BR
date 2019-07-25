---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef4a1a6a820fcb54c86e55824a80e98492bb69c3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/contacts/{id}/getMemberObjects')
    .version('beta')
    .post(String);

```