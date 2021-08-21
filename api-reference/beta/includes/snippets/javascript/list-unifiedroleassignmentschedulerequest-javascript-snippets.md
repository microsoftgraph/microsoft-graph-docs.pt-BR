---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f53b6c49fcf0d9dc75ae376d9008f22665f0245e3a8deff970982b6a2a641ca5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentScheduleRequests = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests')
    .version('beta')
    .get();

```