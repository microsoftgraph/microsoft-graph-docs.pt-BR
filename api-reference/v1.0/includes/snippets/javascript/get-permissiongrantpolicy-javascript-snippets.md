---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faa47226fbc01510593788752926d7dec203959b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .get();

```