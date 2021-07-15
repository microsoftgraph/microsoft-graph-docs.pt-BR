---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e388f020286915a7e5eabaac90658ea8ea5d8860
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentSchedule = await client.api('/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413')
    .version('beta')
    .get();

```