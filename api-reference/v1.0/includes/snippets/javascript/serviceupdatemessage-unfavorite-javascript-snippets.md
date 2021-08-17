---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 991d8b7f1a36fc6ea238b11427142221336a48cf
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/unfavorite')
    .post(_boolean);

```