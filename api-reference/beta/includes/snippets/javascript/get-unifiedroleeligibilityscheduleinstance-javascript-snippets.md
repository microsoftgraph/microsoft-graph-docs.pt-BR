---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33b7d6fb3ff932a99cdd8bcfac3956c009568f45
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleInstance = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances/5cfd7709-7709-5cfd-0977-fd5c0977fd5c')
    .version('beta')
    .get();

```