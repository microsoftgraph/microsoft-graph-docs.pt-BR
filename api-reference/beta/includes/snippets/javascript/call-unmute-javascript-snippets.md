---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75758a04964e6954cdcd25debf6aec543f01a09e
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302784"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unmuteParticipantOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/unmute')
    .version('beta')
    .post(unmuteParticipantOperation);

```