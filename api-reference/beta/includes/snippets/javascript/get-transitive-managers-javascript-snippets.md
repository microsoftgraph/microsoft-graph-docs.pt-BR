---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30099eea9d59af9fe02b8bf8f62fef8781323ba0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .expand('manager($levels=max;$select=id,displayName)')
    .select('id,displayName')
    .get();

```