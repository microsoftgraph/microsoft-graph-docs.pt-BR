---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7312921fb54a9fe579bb6e29c758323e27bc3a96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```