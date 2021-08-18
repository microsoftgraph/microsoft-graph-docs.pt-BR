---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb31dc28024a5fdb057b2d825a5f323f44d0ae24
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266330"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/markRead')
    .post(_boolean);

```