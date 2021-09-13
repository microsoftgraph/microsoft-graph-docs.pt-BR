---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7b9d7e2318631a0fe5708d8282305827a2e9c5142f38192dc9060efb70d1a22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275156"
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

await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments/setOrder')
    .version('beta')
    .post(setOrder);

```