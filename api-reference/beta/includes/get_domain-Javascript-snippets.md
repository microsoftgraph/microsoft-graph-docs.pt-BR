---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c18898eec9384fc38695006dd0f85717f067a2bb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .version('beta')
    .get();

```