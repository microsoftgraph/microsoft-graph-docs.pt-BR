---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a088991f8f62924c665a9720f01942ea4e2956b9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let requests = await client.api('/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests')
    .version('beta')
    .get();

```