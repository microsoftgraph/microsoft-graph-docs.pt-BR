---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f46e9cd406c1bd1195975a77532a2c942d50daa6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  startDateTime: '2019-07-12T14:30:34.2444915-07:00',
  endDateTime: '2019-07-12T15:00:34.2464912-07:00',
  subject: 'User Token Meeting'
};

await client.api('/me/onlineMeetings')
    .post(onlineMeeting);

```