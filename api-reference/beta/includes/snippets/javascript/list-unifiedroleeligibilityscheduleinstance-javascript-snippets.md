---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcafec7356f1cc017d95171a431ceebbde50ce00
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474488"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilityScheduleInstances = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances')
    .version('beta')
    .get();

```