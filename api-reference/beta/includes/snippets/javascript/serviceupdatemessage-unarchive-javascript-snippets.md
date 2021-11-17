---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f04caf1813e3d83b9e77ab97ce3ae8aeb07a4624d2a23db382ccbf4025d8b7b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _boolean = {
  messageIds: ['MC172851', 'MC167983']
};

await client.api('/admin/serviceAnnouncement/messages/unarchive')
    .version('beta')
    .post(_boolean);

```