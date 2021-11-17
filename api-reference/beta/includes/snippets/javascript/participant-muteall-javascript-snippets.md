---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 111028af656eaac9c7ff284dab7df4fd16c53c363abce57805b10af4216be8c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantsOperation = {
  participants: [
    ''
  ],
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/{id}/participants/muteAll')
    .version('beta')
    .post(muteParticipantsOperation);

```