---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c167346fa6ac62c372553d64cb926fbea2d9293f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/devices/{id}/memberOf/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'A\')')
    .orderby('displayName')
    .get();

```