---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49b19dd1144a62850c34828722c151376493617e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause')
    .version('beta')
    .post();

```