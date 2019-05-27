---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07d361280e02243ee45c6bc03d76ae2e827007c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   changeType: "created,updated",
   notificationUrl: "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   resource: "me/mailFolders('Inbox')/messages",
   expirationDateTime:"2016-11-20T18:23:45.9356913Z",
   clientState: "secretClientValue"
};

let res = await client.api('/subscriptions')
    .post({subscription : subscription});

```