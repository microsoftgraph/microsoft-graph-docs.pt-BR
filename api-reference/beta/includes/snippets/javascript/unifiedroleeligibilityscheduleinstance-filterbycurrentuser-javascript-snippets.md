---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee192298340a08d03489dfbc3fa934a6ae70ed73
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances/filterByCurrentUser(on='principal')')
    .version('beta')
    .get();

```