---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b01dfdc97f88e3eb15ba7e91e35e8b5211060f8e36776e14e6e983cc4e41304
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  assignedLabels: 
  [
    {
        labelId: '45cd0c48-c540-4358-ad79-a3658cdc5b88'
    }
  ]
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```