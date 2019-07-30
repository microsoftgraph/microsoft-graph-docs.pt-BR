---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c0010cb3c4699204856ecd0afabdf3a4460de42
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/{id}/mute')
    .version('beta')
    .post(muteParticipantOperation);

```