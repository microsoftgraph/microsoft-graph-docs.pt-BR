---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c5b092e33ffc3d6bb974423a30cbd1e20043d454ea813cb578c1e7fc80cac99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupId-value1', 'groupId-value2' 
  ]
};

await client.api('/contacts/{id}/checkMemberGroups')
    .post(string);

```