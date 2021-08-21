---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce3aa35b8fb99d1714293962d4febd2595de1f8b454f14406fdb2fcdfa638c52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215551"
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