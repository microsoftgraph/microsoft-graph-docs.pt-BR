---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d25d3147e43fdccd21886dad7c172c7aeec3a1a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicies = await client.api('/policies/activityBasedTimeoutPolicies')
    .get();

```