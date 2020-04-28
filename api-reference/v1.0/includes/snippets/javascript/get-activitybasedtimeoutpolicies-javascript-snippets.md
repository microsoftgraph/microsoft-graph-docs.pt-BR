---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb43736249db9156f5aa9b5a145d71ab6bc625bb
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43718462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/activityBasedTimeoutPolicies')
    .get();

```