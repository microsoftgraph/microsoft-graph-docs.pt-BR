---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04072a501b83798b9e9fcbc28f6a558bdfa386a4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies')
    .get();

```