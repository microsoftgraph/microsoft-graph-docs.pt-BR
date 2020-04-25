---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a36471b3dd93133fbff04397e5a19f59c5eaf6d2
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenLifetimePolicies/{id}/$ref')
    .delete();

```