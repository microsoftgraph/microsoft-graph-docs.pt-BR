---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aaac9622b4e23f7853b4838555bf7eede5d10150
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .filter('scopeId eq \'/\' and scopeType eq \'Directory\'')
    .expand('rules')
    .get();

```