---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 807be8a0b209de09cb70e6e6824799ffd9e361ca9b0bea804b819ae1782b5e08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute')
    .version('beta')
    .post(muteParticipantOperation);

```