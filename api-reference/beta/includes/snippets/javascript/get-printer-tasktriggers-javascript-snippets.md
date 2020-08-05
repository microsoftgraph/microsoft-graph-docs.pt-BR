---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e909f04a515d137850af02a32929353d18618c73
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/taskTriggers')
    .version('beta')
    .get();

```