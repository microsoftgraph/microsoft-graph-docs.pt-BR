---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a42958f2e2229508d0c7649715538acbcc63ac0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilityScheduleRequests = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .get();

```