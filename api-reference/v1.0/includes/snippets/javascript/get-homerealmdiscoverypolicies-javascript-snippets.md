---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9c1e4610bb73032364c4376ff7b661d13b6a95b
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/homeRealmDiscoveryPolicies')
    .get();

```