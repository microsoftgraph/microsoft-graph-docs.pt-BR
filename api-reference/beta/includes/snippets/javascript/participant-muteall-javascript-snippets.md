---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ab63cdcbbd9fa4c7ecc5db471bab7b09826ee5a
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantsOperation = {
  participants: [
    ""
  ],
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/{id}/participants/muteAll')
    .version('beta')
    .post(muteParticipantsOperation);

```