---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17e6167de60ad2baec33c125a41edc730177b6a7
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/archive')
    .version('beta')
    .post(_boolean);

```