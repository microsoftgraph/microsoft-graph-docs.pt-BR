---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939b0adbe022a6043d2f92ead156f661d3b2888c
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute')
    .version('beta')
    .post(muteParticipantOperation);

```