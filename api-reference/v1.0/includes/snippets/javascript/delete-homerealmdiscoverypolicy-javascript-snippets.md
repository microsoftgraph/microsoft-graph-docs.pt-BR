---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73af7451d882ee94dd2aed6db5e53e14859bee0e
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .delete();

```