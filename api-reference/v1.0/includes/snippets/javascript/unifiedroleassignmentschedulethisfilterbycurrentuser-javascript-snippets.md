---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 436625cae67115a8443ab4aaeafb0034a5bcd145
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleAssignmentSchedules/filterByCurrentUser(on='principal')')
    .get();

```