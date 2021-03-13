---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 695f86664f57a53b4ecc6eefd2bc598de8a89949
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  lobbyBypassSettings: {
      isDialInBypassEnabled: true
  }
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi')
    .update(onlineMeeting);

```