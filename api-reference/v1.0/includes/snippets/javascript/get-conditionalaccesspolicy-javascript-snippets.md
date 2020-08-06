---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3f3e5640e1712c94674ac8d347100d1f95b678e
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies/{id}')
    .get();

```