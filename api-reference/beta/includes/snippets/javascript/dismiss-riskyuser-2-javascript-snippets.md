---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3acbab296d7cb6ada4941c2dd6237ba1733317b7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    '04487ee0-f4f6-4e7f-8999-facc5a30e232'
  ]
};

await client.api('/identityProtection/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```