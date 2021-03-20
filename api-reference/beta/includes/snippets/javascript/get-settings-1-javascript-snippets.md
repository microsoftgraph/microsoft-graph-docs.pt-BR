---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 207d8153410f71b313f2d0f6c9422a10af39e362
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946521"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/settings')
    .version('beta')
    .get();

```