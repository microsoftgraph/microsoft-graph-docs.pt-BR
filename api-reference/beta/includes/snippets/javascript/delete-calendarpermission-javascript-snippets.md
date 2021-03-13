---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd5b779c6a6d86915a426021f46611d1919092f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/calendar/calendarPermissions/{id}')
    .version('beta')
    .delete();

```