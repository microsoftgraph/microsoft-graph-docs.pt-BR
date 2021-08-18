---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 996a02f71318abc6d5c450b5ae60e52b7637b13db784d24edc7d64dab0b600f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215574"
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
    .version('beta')
    .update(onlineMeeting);

```