---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1915254a116a45ab7c890567a52c77d0f1b83c2b
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances/filterByCurrentUser(on='principal')')
    .version('beta')
    .get();

```