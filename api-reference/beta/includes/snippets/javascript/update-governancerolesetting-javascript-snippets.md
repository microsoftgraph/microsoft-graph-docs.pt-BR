---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a68851b68996c90b50c2b00856ab2d7c6dab0d94
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleSetting = {
   adminEligibleSettings:[
      {
         ruleIdentifier:"ExpirationRule",
         setting:{\"permanentAssignment\:false,\maximumGrantPeriodInMinutes\:129600}"
      }
   ]
};

let res = await client.api('/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5')
    .version('beta')
    .update({governanceRoleSetting : governanceRoleSetting});

```