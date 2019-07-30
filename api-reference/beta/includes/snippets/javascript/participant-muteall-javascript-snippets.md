---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27d2bdb1408da501295c02d96912d7b1f42e5ac7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933778"
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

let res = await client.api('/app/calls/{id}/participants/muteAll')
    .version('beta')
    .post(muteParticipantsOperation);

```