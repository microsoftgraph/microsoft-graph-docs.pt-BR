---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f29684b0302ddae42c032c8a0783c54d241e1f1e
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .get();

```