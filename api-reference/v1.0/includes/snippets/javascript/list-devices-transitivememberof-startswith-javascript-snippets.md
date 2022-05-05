---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed533d9e54698dc5232cefcf72a7e82b29416500
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/devices/{id}/transitiveMemberOf/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .orderby('displayName')
    .get();

```