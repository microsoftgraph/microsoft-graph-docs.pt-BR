---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7a27218d03b402c9246a3b410d7c1268a35072c
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476115"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .delete();

```