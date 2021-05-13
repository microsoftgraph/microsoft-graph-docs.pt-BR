---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 379af850e79f311bc2a0deadd763982aa47f9cea
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleScheduleInstances = await client.api('/roleManagement/directory/roleScheduleInstances(directoryScopeId='parameterValue',appScopeId='parameterValue',principalId='parameterValue',roleDefinitionId='parameterValue')')
    .version('beta')
    .get();

```