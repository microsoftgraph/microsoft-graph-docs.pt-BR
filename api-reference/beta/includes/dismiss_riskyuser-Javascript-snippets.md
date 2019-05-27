---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 525f3819a68e79648494f692bb5d79e6cbef2dcd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  userIds: [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
};

let res = await client.api('/riskyUsers/dismiss')
    .version('beta')
    .post(dismiss);

```