---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7e6abfdf5be941c8f3a129e758357c69141ec85
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .header('ConsistencyLevel','eventual')
    .expand('manager($levels=max;$select=id,displayName)')
    .select('id,displayName')
    .get();

```