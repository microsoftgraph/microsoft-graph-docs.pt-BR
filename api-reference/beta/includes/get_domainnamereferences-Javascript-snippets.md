---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 300aa93262e375366c3b9a400fb9f63c4c3c8874
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/domainNameReferences')
    .version('beta')
    .get();

```