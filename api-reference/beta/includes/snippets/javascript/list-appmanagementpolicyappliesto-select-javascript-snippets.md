---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9914ad70e1cb1c19fa4723ed3bb9909a5bc8db50
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appliesTo = await client.api('/policies/appManagementPolicies/{id}/appliesTo')
    .version('beta')
    .select('id,appId,displayName,createdDateTime')
    .get();

```