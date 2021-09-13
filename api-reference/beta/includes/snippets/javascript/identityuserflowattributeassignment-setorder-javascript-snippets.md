---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f135587fb3ff2826dd73a30601654ce168a25edf2768832dce6054201508f680
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setOrder = {
  newAssignmentOrder: {
    order: [
        'City',
        'extension_GUID_ShoeSize'
    ]
  }
};

await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder')
    .version('beta')
    .post(setOrder);

```