---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 162f231cfbfb31cecbb5c783986a645ca652c200
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206532"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .get();

```