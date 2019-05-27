---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46441219b5773b9cce9aa76aa37e89c80b3a00c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .version('beta')
    .get();

```