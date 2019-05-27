---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf2af8d025c2f2ada9b6e1ecdff3a3e82e819d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive')
    .get();

```