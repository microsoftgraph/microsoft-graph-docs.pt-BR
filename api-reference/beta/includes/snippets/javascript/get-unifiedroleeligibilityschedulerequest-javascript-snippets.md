---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36198fcbf0d3def00e0757d89d739a8c49162dcf
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleRequest = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/26bc6813-5457-4302-a482-afafd4e2962a')
    .version('beta')
    .get();

```